---
owner_slack: "#operations-engineering-alerts"
title: How to be Support
last_reviewed_on: 2023-12-04
review_in: 3 months
---

# How to be Support

This document will guide you on what to do while on 'Support'.

## What is Support?

Support is a role within the team responsible for responding to customer queries and requests, as well as several monitoring tasks.
All team members are expected to contribute to the support rota and be available to respond to customer queries and requests.

While an individual is on support at any given time, the team is expected to contribute and be available to assist wherever possible.

## How do we know who's on support?

The support rota is published on the [team calendar](https://calendar.google.com/calendar/embed?src=c_rqkd9jdtg9kgditulka4ocit78%40group.calendar.google.com&ctz=Europe%2FLondon).

## What's expected of us on support?

Note: This list is not exhaustive and is subject to change. It was gathered during a Slack conversation and is meant to be a starting point for discussion.

    `1. Respond to customer queries and requests`

The [#ask-operations-engineering](https://mojdt.slack.com/archives/C01BUKJSZD4) Slack channel is our primary channel for customer queries and requests.
Monitor this channel and respond to queries and requests as they come in. If you need to know something, ask the team.

    `2. Monitor the support inbox`

There are many email groups you should monitor for customer queries and requests. They are:

- [Ops Eng Google Group](https://groups.google.com/a/digital.justice.gov.uk/g/operations-engineering)
- [Domains Google Group](https://groups.google.com/a/digital.justice.gov.uk/g/domains)
- [Certificates Google Group](https://groups.google.com/a/digital.justice.gov.uk/g/certificates)
- [Certificates Alerts Google Group](https://groups.google.com/a/digital.justice.gov.uk/g/certificate_alerts)

If a request comes in on the day you're on support, please do it unless the email is a follow on from a previous request.

Add the `closed` label to the email when you've completed the required action.

A few examples of the types of requests you'll receive in these mailboxes are:

- [Respond to certificates that have expired/about to expire](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/certificates/respond-to-expired-certs.html)
- [Respond to leavers forms and remove their access](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/internal/respond-to-leavers.html)

  `3. Review the documentation that has expired`

Documentation in Operations Engineering is reviewed regularly.
If a document was reviewed over 3 months ago, it should be reviewed again. Expired documentation will appear in the #operations-engineering-alerts slack channel.

We use [Daniel the Manual Spaniel](https://technology.blog.gov.uk/2020/09/25/keeping-tech-docs-up-to-date-with-daniel-the-manual-spaniel/)
to monitor our documentation. If a document has expired, it will be flagged in the #operations-engineering-alerts Slack channel.
Please review the document and raise a PR to update it when you see this. When finished, add a tick emoji to the Slack message.

    `4. Monitor and review PRs in the Collaborators repository`

The [Collaborators repository](https://github.com/ministryofjustice/github-collaborators/pulls) manages
third-party access to our GitHub repositories. If a PR is raised, review it and contact the repository owner to confirm the request.

If we have several requests simultaneously, close them and add them to a single PR.

You can read more about the [collaborators process here](https://github.com/ministryofjustice/github-collaborators/blob/main/README.md).

    5. Monitor the #operations-engineering-alerts slack channel

The #operations-engineering-alerts Slack channel is used to notify the team of any issues that must be addressed.
If a major service is down (used by approximately 50% of users), send communication to the #operations-engineering-update slack channel.

## How do we volunteer for support?

During standup, inform the team you'd like to be the support person for the day.
