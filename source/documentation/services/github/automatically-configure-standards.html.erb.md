---
owner_slack: "#operations-engineering-alerts"
title: Automatically configure GitHub Repository Standards
last_reviewed_on: 2023-08-31
review_in: 3 months
---

# Automatically configure GitHub Repository Standards

There are a set of [standards](https://operations-engineering.service.justice.gov.uk/documentation/services/repository-standards.html) that all GitHub repositories inside the Ministry of Justice GitHub Organisations should abide by.

## What does the automation do?

Operations Engineering maintains automation that can configure and maintain these standards for you.

Standards the automation configures:

* Default Branch Protection
* Enforce Admins
* Required Review Count
* Dismiss Stale Reviews
* Enable Issues

Standards the automation does not currently configure:

* Description set
* License

## How do I use the automation?

In order to enable the automation for a given GitHub repository, follow these steps:

1. Navigate to the Repository page
2. Click the Cog on the top right of the page
3. Add a new topic called "standards-compliant"
4. Save the changes

## How do I turn off the automation?

In order to disable the automation for a given GitHub repository, follow these steps:

1. Navigate to the Repository page
2. Click the Cog on the top right of the page
3. Remove the "standards-compliant" topic
4. Save the changes

## When does the automation run?

Currently the automation runs at 6am every day and can be run manually [here](https://github.com/ministryofjustice/operations-engineering/actions/workflows/configure-standards.yml)

## Things to note

A few things to note if enabling the automation:

* It will overwrite any changes you make that go against the standards
* If new standards are added, it will automatically attempt to configure them