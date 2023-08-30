---
owner_slack: "#operations-engineering-alerts"
title: Listing Hosted Zones not in Terraform/DNS-IAC
last_reviewed_on: 2023-08-30
review_in: 3 months
---

# Listing Hosted Zones not in Terraform/DNS-IAC

[DNS-IAC](https://github.com/ministryofjustice/dns-iac) contains a record of the AWS DSD Route53 estate, however for a number of reasons (mainly API limits), not everything is in the code.

The DNS IAC repository contains a [script](https://github.com/ministryofjustice/dns-iac/blob/main/scripts/get-zone-drift.py) that prints out the difference between DNS-IAC and Route53 in terms of Hosted Zones.

## Requirements

The script is run from the command prompt, the following requirements are needed:

- Python3
- boto3 Python3 lib
- Terraform
- Authentication to the DSD AWS account (this contains the Route53 records)
- It is recommended you have at least a basic knowledge of general Programming, Terraform and Route53.

> A pip [requirements](https://github.com/ministryofjustice/dns-iac/blob/main/scripts/requirements.txt) file is present for quick installation.

Drift within DNS-IAC is when manual changes are made to the DSD Route53 configuration and not reflected within the DNS-IAC codebase. Essentially it is when what Terraform expects and what Route53 has is different.

## Running the script

1. Clone the DNS IAC repository (<https://github.com/ministryofjustice/dns-iac>)
2. Open the script file (<https://github.com/ministryofjustice/dns-iac/blob/main/scripts/create-zone.py>)
3. Edit the following line so that `ZONE_NAME` is equal to the AWS Route53 Hosted Zone name you wish to add e.g. dsd.io, gov.uk etc
4. Ensure you are authenticated against the DSD AWS account and run the Python script

This will create the relevant Terraform files and print to console a list of instructions you will need to run

5. Run the instructions IN ORDER printed to the console by the script previously
6. Run Terraform plan to ensure there is no drift and everything has been imported successfully (Terraform should report no changes needed)
7. Create PR with the new Terraform files generated and merge into main