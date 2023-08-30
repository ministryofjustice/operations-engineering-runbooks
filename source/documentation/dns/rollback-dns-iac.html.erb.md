---
owner_slack: "#operations-engineering-alerts"
title: Rolling back DNS-IAC
last_reviewed_on: 2023-08-30
review_in: 3 months
---

# Rolling back DNS-IAC

> Please be careful when doing this process, if you do not understand Terraform and the AWS DSD R53 estate, seek guidance from someone that does

There can be cases when you wish to rollback any changes made to AWS Route53 using DNS-IAC, this document includes the process for that.

> Be aware this process is new and this page may not cover unexpected steps, please update the process accordingly.

# The process

In order to rollback DNS-IAC the high level process is as follows:

> A laptop authenticated against the DSD AWS account is needed for this process

1. Checkout DNS-IAC

```
git checkout https://github.com/ministryofjustice/dns-iac.git
```

2. Checkout the commit you wish to revert to

```
cd dns-iac && git checkout $commit_hash
```

3. Run terraform plan on a laptop authenticated against the DSD AWS account

```
terraform plan
```

4. Check the changes in Terraform are the ones you wish to revert

> Please be careful when doing this - this can be a very contextual area, you need up to date knowledge of the Route53 estate

5. Run Terraform apply

```
terraform apply -auto-approve
```

6. Revert to the target commit

```
git revert --no-commit $commit_hash..HEAD
git commit -m "Revert $commit_hash"
git push
```

8. Open up a PR to merge in the revert