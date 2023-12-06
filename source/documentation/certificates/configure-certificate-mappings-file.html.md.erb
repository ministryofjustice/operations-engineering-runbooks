---
owner_slack: "#operations-engineering-alerts"
title: Configuring the Certificate Mappings File
last_reviewed_on: 2023-09-27
review_in: 3 months
---

# Configuring the Certificate Mappings File

## Overview

This document describes how to edit the certificate mappings file on AWS to determine which email addresses are informed about any expiring certificates managed by Operations Engineering.

The mappings file in question is in JSON format. It is used by the [operations-engineering-certificate-renewal](https://github.com/ministryofjustice/operations-engineering-certificate-renewal) repository to identify the correct group email address to send these notifications to.

The file itself sits in an S3 bucket, which can be found [here](https://s3.console.aws.amazon.com/s3/buckets/operations-engineering-certificate-email?region=eu-west-2&tab=objects). The current file in use is named `mappings.json` - the `cjscp_hmcts_mappings.json` is a list of all certs managed by either CJSCP or HMCTS in the same format; this is current not being used.

Here is an example of an entry in the file, with a breakdown of each field:

```
  "example.domain.com": {
    "recipient": "example-email@justice.gov.uk",
    "recipientcc": [
      "another-example-email@justice.gov.uk"
    ],
    "owner": "OE",
    "external_cname": []
  }
```

| Field              | Description                                                                                                                                            |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| example.domain.com | This is where the domain name in question sits, all information below it is attributed to that domain.                                                 |
| recipient          | The primary email address to send the notification to.                                                                                                 |
| recipientcc        | Any additional email addresses to send the notification to can be defined here, should they be needed.                                                 |
| owner              | Which team manages the certificate (OE, CJSCP, HMCTS).                                                                                                 |
| external_cname     | Contains the email address associated with adding CNAME records to hosted zones outside of Operations Engineering's remit. This is currently not used. |

More information on the certificate renewal process can be found in the [Renewing an expiring certificate via Gandi.net](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/certificates/manual-ssl-certificate-processes.html#renewing-an-expiring-certificate-via-gandi-net) section of the certificate processes runbook.

## Editing the Mapping File

Occasionally, we may need to modify what is in the mappings file. This could be modifying the email address associated with a domain or removing an entry entirely.

It isn't possible to edit the file directly from the S3 bucket it's stored in, so please follow the below steps if you need to make any changes. Before you do it, checking that the notification action isn't due to run to avoid errors is worth checking. Currently, it's set up to run daily at 10:00 am.

1. Navigate to the mappings file on AWS. This is located [here](https://s3.console.aws.amazon.com/s3/object/operations-engineering-certificate-email?region=eu-west-2&prefix=mappings.json).
2. Download a copy of the file.
3. Rename the mappings file within the S3 bucket to something like `mappings_old.json`.
4. Make the required changes to the file.
5. Reupload the file to the S3 bucket. The file **must** be called `mappings.json`.

The `mappings_old.json` file can be deleted from the bucket whenever; however, waiting until at least one successful run of the notification action is recommended to ensure everything is working as expected.
