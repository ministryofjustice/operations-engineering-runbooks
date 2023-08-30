---
owner_slack: "#operations-engineering-alerts"
title: How to manually recover deleted DNS records
last_reviewed_on: 2023-08-29
review_in: 3 months
---

# How to manually recover deleted DNS records

## Overview

The purpose of this runbook is to provide instructions for reverting DNS changes if you don't have a back-up or DNS is not captured in [DNS-IAC](https://github.com/ministryofjustice/dns-iac).

## Recovering DNS from Cloudtrial logs

If you don't have a backup or if DNS isn't captured in DNS-IAC, you can [recover records from the Cloudtrail logs](https://aws.amazon.com/premiumsupport/knowledge-center/route-53-recover-dns-record/).

You can then find the DNS records to restore from the JSON output.