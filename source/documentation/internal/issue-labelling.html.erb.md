---
owner_slack: "#operations-engineering-alerts"
title: Issue Labelling
last_reviewed_on: 2023-09-01
review_in: 3 months
---

# Issue Labelling

## Purpose

This runbook sets out our approach for labelling Issues.

[Labels](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels) is a feature that makes it easier to understand more about an Issue at a glance. They are also a good way of sorting or filtering Issues.

A story type Issue will typically have 4 labels assigned to it:

**Product/Service** - This identifies which product or service the story relates to e.g. `GitHub`

**Workflow Status** - This identifies where an Issue is in our delivery workflow and helps the team know if a story can be worked on or not e.g. `Needs Refining` (i.e. the story is not yet ready to be worked on).

**MoSCoW Priority** - This helps identify priority using the [MoSCoW system](https://www.productplan.com/glossary/moscow-prioritization/#:~:text=The%20acronym%20MoSCoW%20represents%20four,MoSCoW%20to%20mean%20%E2%80%9Cwish.%E2%80%9D). This label will normally be agreed during Backlog Refinement or Planning e.g. `Must Have` (i.e. mandatory user need)

**Type of Story** - This indicates the principle type of work that the story might involve e.g. `Documentation` (e.g. the story is for creating a runbook)

**Language** - Idetifies coding language required to complete this story. Only applies to `Development` "Type" stories

## Exceptions

There are two exceptions for labelling Issues:

**Support Issues** - These are automatically updated with the `Support` Label. When you raise a support Issue you should manually add the appropriate "Product" label.

**GitHub Feature Requests** - These are automatically updated with the `feature request`, `github` and `third party` labels.

## Available Labels for Story type Issues

| Product/Service | Workflow Status | MoSCoW Priority | Type of Story | Language |
|-----------------|-----------------|-----------------|---------------|----------|
| 1Password | Needs Refining | Must Have | Community | Ruby |
| Auth0 | Refined | Should Have | Documentation | Python |
| CircleCI | Agreed for Sprint | Could Have | EPIC | Terraform |
| DNS-IAC | Purged | Wont Have | Feature Request | |
| Docker | Blocked |  | Policy | |
| Domain Management | Unplanned |  | Spike | |
| Github | | | Support | |
| Github actions | | | User Research | |
| Maintenance Pages | | Development | |
| OS Data Hub APIs | | | |
| Other Support Request | | | |
| PagerDuty | | | |
| Pingdom | | | |
| Sentry | | | |
| SonarCloud.io | | | |
| SSL Certificate Management | | | |
| Standards | | | |
| Tech Docs | | | |
| AWS Root Account | | | |
