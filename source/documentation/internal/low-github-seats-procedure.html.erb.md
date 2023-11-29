---
owner_slack: "#operations-engineering-alerts"
title: Low GitHub Seats Response Procedure
last_reviewed_on: 2023-11-29
review_in: 3 months
---

# Low GitHub Seats Response Procedure

## Overview

This document outlines the steps to follow when an alarm is triggered in our Slack channel, indicating potential issues with dormant users or low GitHub seats.

## Steps to Follow

### Initiate Dormant Users Process:

On receiving an alarm in Slack, start the "Dormant Users" process as described in our [runbook](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/internal/dormant-user-process.html).

### Retrigger GitHub Action:

After completing the Dormant Users process, retrigger the "check-for-low-github-seats" GitHub action to reassess the seat count.

If the GitHub action retriggers the alarm, indicating a continued issue with low GitHub seats, contact Steve or Tony.
