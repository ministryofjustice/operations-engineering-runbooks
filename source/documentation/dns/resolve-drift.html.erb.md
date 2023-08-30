---
owner_slack: "#operations-engineering-alerts"
title: Resolving Drift for DNS-IAC
last_reviewed_on: 2023-06-14
review_in: 3 months
---

# Resolving Drift for DNS-IAC

Drift within DNS-IAC is when manual changes are made to the DSD Route53 configuration and not reflected within the DNS-IAC codebase. Essentially it is when what Terraform expects and what Route53 has is different.

This difference can cause problems such as:

- Reverting changes made in Route53
- Making unwanted changes in Route53
- Making it impossible to rollback in the case of a failed release
- Making it impossible to make further changes without significant troubleshooting

This runbook provides a set of steps that should be followed to ensure there is no drift between DNS-IAC and Route53.

## Is there Drift?

In order to identify if there is drift, you can do either of the following actions:

1. Run the [Terraform plan workflow](https://github.com/ministryofjustice/dns-iac/actions/workflows/terraform-plan.yml)
2. Run `terraform plan` on a laptop authenticated against the DSD AWS account from the `main` repository branch

Both of the above processes should produce a Terraform plan, the expected result should be as follows:

`No changes. Your infrastructure matches the configuration.`

If the above message is not given at the end of the Terraform plan output, there is drift - an example of the output with drift is as follows:

`Plan: 5 to add, 4 to change, 6 to destroy.`

## Fixing Drift

> Please be careful when doing this - this can be a very contextual area, you do need to up to date knowledge with planned changes in the Route53 estate

In order to fix drift, you must change the DNS-IAC Terraform code to match the current Route53 configuration.

1. Firstly confirm that everything in the `main` repository branch has previously been applied to Route53, if someone has forgot to apply this may look like drift but infact are actually wanted changes - this should not be an issue once we add apply to the CICD pipeline.
2. Once confirmed that all wanted changed have been pushed, refer to the Terraform plan output.
3. Going through each changed resource, change the relevant Terraform code to match what is currently in Route53.
4. Run a `terraform apply`

### An example

Below is a resource from a Terraform plan output, Terraform wants to change `-all` to `~all` (see the - and + on the left hand side)

```
  # module.publicguardian_gov_uk_records.aws_route53_record.this["publicguardian.gov.uk_TXT"] will be updated in-place
  ~ resource "aws_route53_record" "this" {
        id      = "Z01126121SKXV1BMJWB6J_publicguardian.gov.uk_TXT"
        name    = "publicguardian.gov.uk"
      ~ records = [
          + "v=spf1 ip4:redacted ip4:redacted  include:redacted ~all",
          - "v=spf1 ip4:redacted ip4:redacted  include:redacted -all",
            # (1 unchanged element hidden)
        ]
        # (4 unchanged attributes hidden)
    }
```

In order to match the code with what is inside AWS, you first navigate to the file that holds the code, in this case it is `terraform/publicguardian.gov.uk.tf`.

Once the file is open, change the relevant code

```
   {
      name = "publicguardian.gov.uk"
      type = "TXT"
      ttl  = 300
      records = [
        "MS=ms49968440",
        "v=spf1 ip4:redacted  ip4:redacted  include:redacted  ~all"
      ]
    },
```

Would become (`~all` becomes `-all`)

```
   {
      name = "publicguardian.gov.uk"
      type = "TXT"
      ttl  = 300
      records = [
        "MS=ms49968440",
        "v=spf1 ip4:redacted  ip4:redacted include:redacted  -all"
      ]
    },
```