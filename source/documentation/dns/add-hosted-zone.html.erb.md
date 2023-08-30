---
owner_slack: "#operations-engineering-alerts"
title: Importing a Hosted Zone from AWS into DNS-IAC
last_reviewed_on: 2023-08-29
review_in: 3 months
---

# Importing a Hosted Zone from AWS into DNS-IAC

Adding a new Hosted Zone from AWS as code into [DNS-IAC](https://github.com/ministryofjustice/dns-iac) manually can take a long time and has much room for human error.

The DNS IAC repository contains a [script](https://github.com/ministryofjustice/dns-iac/blob/main/scripts/create-zone.py) that automates this process.

## Requirements

The script is run from the command prompt, the following requirements are needed:

- Python3
- boto3 Python3 lib
- Jinja2 Python3 lib
- Terraform
- Authentication to the DSD AWS account (this contains the Route53 records)
- It is recommended you have at least a basic knowledge of general Programming, Terraform and Route53.

> A pip [requirements](https://github.com/ministryofjustice/dns-iac/blob/main/scripts/requirements.txt) file is present for quick installation.

## Running the script

1. Clone the DNS IAC repository (<https://github.com/ministryofjustice/dns-iac>)
2. Ensure you are authenticated with the DSD AWS Account and run the script file (<https://github.com/ministryofjustice/dns-iac/blob/main/scripts/create-zone.py>)

The console will output the following infomation:

1. All Hosted Zones that are not in Terraform (reverse drift)
2. All Hosted Zones that are in Terraform but no longer in AWS