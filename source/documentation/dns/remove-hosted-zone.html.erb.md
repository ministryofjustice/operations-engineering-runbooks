---
owner_slack: "#operations-engineering-alerts"
title: Removing a Hosted Zone using DNS IAC
last_reviewed_on: 2023-08-30
review_in: 3 months
---

# Removing a Hosted Zone using DNS IAC

Removing a new Hosted Zone from AWS using [DNS-IAC](https://github.com/ministryofjustice/dns-iac) can often be part of a domain decommissioning process.

This document walks through the steps needed to do this.

## Requirements

The following requirements are needed:

- Terraform
- Authentication to the DSD AWS account (this contains the Route53 records)
- It is recommended you have at least a basic knowledge of general Terraform and Route53.

## Steps required

1. Clone the DNS IAC repository (<https://github.com/ministryofjustice/dns-iac>)
2. Ensure you are authenticated with the DSD AWS Account and then run `terraform init` and then `terraform apply`
3. Confirm there is no drift after the Terraform plan has finished, if there is, this must be resolved first: [Resolve Drift](resolve_drift.html)
4. Remove the Hosted Zone Terraform file from the Terraform directory in the DNS IAC repository
5. Run `terraform init` and then `terraform apply`
6. Create a PR and merge the removed file/s into main