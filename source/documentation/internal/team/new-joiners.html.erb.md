---
owner_slack: "#operations-engineering-alerts"
title: New Joiners Guide
last_reviewed_on: 2024-05-07
review_in: 3 months
---

# New Joiners Guide

When a new team member joins, follow this guide, and log completion in a ticket. You need to be a civil servant to complete the steps that require ServiceNow.

## Order MacBook / Kit

To get a MacBook (e.g. for a new starter), order it in ServiceNow, by searching for “Mac” (not MacBook!).
[Service Now "Mac" Search](https://mojprod.service-now.com/moj_sp?id=search&spa=1&t=moj_sc&q=mac)

## Request Google Workspace

[Service Now](https://mojprod.service-now.com/moj_sp?id=sc_cat_item&sys_id=fc4dcab3db50a09050fbbfce3b96194b)

## Slack

[Slack tasks for the D&T Workspace](https://mojprod.service-now.com/moj_sp?id=search&spa=1&t=moj_sc&q=mac)

Add new team members to `#operations-engineering-team`, `#operations-engineering-alerts`, `#ask-operations-engineering` and `#analytical-platform-support`.

## Ops-Engineering site

This [site](https://user-guide.operations-engineering.service.justice.gov.uk/#moj-operations-engineering-user-guides) explains the Tools below. Details of vision for team, how we work, all our services, code and runbooks.

## Technical Guidance site

This [site](https://technical-guidance.service.justice.gov.uk/) has additional technical information and decisions.

## Github Account

Setup a new account on [Github](https://github.com/) or assign the digital justice email to your account and make it the primary email so that emails go to that email address.

## MoJ Github

Runbook: [Add user to GitHub](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/services/github/add-github-user.html)

After the invitation has been accepted, check access to the [Ministry of Justice organisation](https://github.com/ministryofjustice) and the [moj-analytical-services organisation](https://github.com/orgs/moj-analytical-services).

Ask an existing team member to bump your account to a GitHub Owner.

Join the the operations-engineering team on both Organisations.

## Access to project board(s)

We use the [Operations Engineering GitHub Project](https://github.com/orgs/ministryofjustice/projects/52) to manage our workflow.

## Access to Miro

Go to [Miro](https://miro.com/) and sign in using Google account. If it asks which project to join from a long list pick "Operations Engineering". If it asks you to make a team create a random name team, then on the left hand side bar is a plus option to pick a project. Alternatively use the link to the [board](https://miro.com/app/board/o9J_l-rEXm0=/)

A google account will enable log-ins to some/most of these tools MOJ provision however some may require licences to use full suite of apps ( e.g Miro for creating boards etc..).

## Tooling for Local Development  

New developers are recommended to have the following tools installed:

- Homebrew
- Python 3.11
- Docker
- Docker Compose
- VSCode
- kubectl
- Terraform
- AWS CLI

This can be achieved by running the following script:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" \
&& brew install --cask python@3.11 \
&& brew install --cask docker \
&& brew install docker-compose \
&& brew install --cask visual-studio-code \
&& brew install kubernetes-cli \ 
&& brew install tfenv \
&& tfenv install latest
```

## 1Password

A team member will send you an email invite to join 1Password.

Runbook: [Add New Users to 1Password](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/services/1password/1password-add-new-user.html)

Add to **Administrators** Group.

## AWS (MoJDSD)

[SSO using GitHub](https://moj.awsapps.com/start)

## Cloud Platform

Access controlled by addition to [Ops Eng GitHub Team](https://github.com/orgs/ministryofjustice/teams/operations-engineering).

## Google Groups

A team member will assign a new Google Group to your Google account:

- Ops Eng Google Group
- Certificates Google Group
- Certificate Alerts Google Group
- Domains Google Group

## Google Drive

Adding team members to the Ops Eng Google Group should automatically add users to the shared Google Drive. If not, add new team members [here](https://drive.google.com/drive/u/1/folders/1Z4z-kNrD-zmwoHmwQaR1-WERo2S1sImX)

## OS DataHub

Admin sets up the account, you will receive an email invite from Ordnance Survey, select the Government user option.

## [Gandi.net](https://www.gandi.net/en-GB)

Admin sets up the account, you will receive an email invite from Gandi.

## [Sentry.io](https://sentry.io/)

Ask an existing member to bump your account to Owner within your profile in the Members section. Use this link to to join Sentry using SSO [GitHub](https://sentry.io/auth/login/ministryofjustice/)

## Pingdom

Access is via a shared user account that is stored in the shared area of passwords in LastPass.

## PagerDuty

Creds in Ops Eng Folder in LastPass. Will be in the shared area of passwords.

## Docker

Runbook: [Add user to Docker](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/services/docker/add-docker-user.html)

## [Auth0](https://auth0.com/)

Use SSO via GitHub to sign in.

Ask an existing member to bump your account to Owner by adding you to the owners team.

## Ops-Eng Team Google Calendar

Use [this invitation link](https://calendar.google.com/calendar/u/0?cid=Y19ycWtkOWpkdGc5a2dkaXR1bGthNG9jaXQ3OEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t) to join the teams Google Calendar.

Alternatively, ask an existing member to open the [settings](https://calendar.google.com/calendar/u/0/r/settings/calendar/Y19ycWtkOWpkdGc5a2dkaXR1bGthNG9jaXQ3OEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t) for the team calendar and add you to the user section.

## Share MoJ Digital Guide

Share this link: <https://docs.google.com/document/d/1KvreqmI_P6E7YLpdRrjefv1fo6B3-B6JBz4MAGiL0Jw/edit#heading=h.33v5b0ui54nd>
