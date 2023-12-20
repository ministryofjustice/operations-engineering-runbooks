---
owner_slack: "#operations-engineering-alerts"
title: Incident Log
last_reviewed_on: 2023-12-19
review_in: 3 months
---

# Incident Log

This is a log of Operations Engineering managed incidents.

## Q4 2023 (October to Decmeber)

- **Mean Time to Repair**: 83h 50m

- **Mean Time to Resolve**: TBC

### Incident on 2023-12-15 - Sentry Session Replay Quota Exhausted

- **Key events**

  - First detected: 2023-12-15 15:34
  - Repaired: 2023-12-15 16:16
  - Resolved: TBC

- **Time to repair**: 0h 42m
- **Time to resolve**: TBC

- **Identified**: Automated alert email from Sentry Support at 80% and 100% Replay quota consumption.
- **Impact**: This resulted in no further Replays being available to any projects until the monthly subscription resets on 14th January 2024.

- **Context**:

  - 2023-12-15 15:34 Email alert from Sentry notifying us that 80% of replay quota exhausted.
  - 2023-12-15 16:16 Notification to users via #operations-engineering-update that quota was due to run out. No further resolution until quota increased.
  - 2023-12-15 22:37 Email alert from Sentry notifying us that 100% of replay quota exhausted.

- **Resolution**: Users notified that quota exhaused and actiomn that is being taken to increase quota.

- **Review Actions**:

N/A - Only action that will resolve furter incidents is an increase in quota, which is already underway.


### Incident on 2023-12-08 - obr.uk email migration - Email failure due to cached MTA-STS policy

- **Key events**

  - First detected: 2023-12-08 14:12
  - Repaired: 2023-12-12 15:18
  - Resolved: 2023-12-12 15:18

- **Time to repair**: 97h 6m
- **Time to resolve**: 97h 6m

- **Identified**: Reported by Email Migration Team.
- **Impact**: Emails not delivered.

- **Context**:

  - 2023-12-08 14:12 HM Treasury (HMT) Email Team report that emails being blocked by unknown MTA-SYS policy.
  - 2023-12-08 15:25 MTA-STS policy removed by Operation Engineering.
  - 2023-12-09 14:15 HMT Email Team report that some email is being delivered. Email via Google still being blocked.
  - 2023-12-10 10:30 HMT Email Team report that email appears to be blocked by a cached MTA-STS policy. Cache based on a policy `max_age` of 14 days. Partial delivery of emails.
  - 2023-12-10 11:08 Original MTA-STS policy reinstated with a short `max_age` to try and clear cached policy.
  - 2023-12-11 10:30 Technical call held to discuss options as email still only being partially delivered. Reinstating policy did not resolve issue. Decision taklen to implement a new `none` type policy.
  - 2023-12-11 10:43 New policy deployed
  - 2023-12-11 14:00 Technical call held. Email still being partially delivered due to cached policy. Decision made to add old MX record server back to see inpact on the policy.
  - 2023-12-11 14:40 HMT Email Team start seeing Non-Delivery Report (NDR) errors. Decision made to revert MX record changes and remove old mail servers. NDR errors stop.
  - 2023-12-12 12:00 Technical call held. Identifed that `max_age` value should be at least 24 hers for some email providers to recognise policy changes. 
  - 2023-12-12 13:05 New MTA-STS policy deployed
  - 2023-12-12 15:18 HMT Email Team report that emails no longer blocked by orginal MTA-STS policy. Email service working as expected.

- **Resolution**: Implementation of new `none` type MTA-STS policy with 24hr `max_age` and no associated MX records resulted in cached policy being replaced. This enabled email to be delivered as expected.

- **Review Actions**:
  - Update Readme to include correct decommissioning actions - **DONE**
  - Create runbook to help assess DNS changes required for email migrations - **TODO**
  - Review of current MTA-STS Infrastucture as Code solution and process to feed into longer terms strategy for this product i.e. tactical uplift vs tackling longer term technical dept.


### Incident on 2023-11-17 - Sentry Session Replay Quota Breach

- **Key events**

  - First detected: 2023-11-17 09:21
  - Repaired: 2023-11-17 15:45
  - Resolved: TBC

- **Time to repair**: 6h 24m
- **Time to resolve**: TBC

- **Identified**: Automated alert email from Sentry Support at 80% and 100% Replay quota consumption.
- **Impact**: This resulted in no further Replays being available to any projects until the monthly subscription resets on 14th December 2023. There are only 3 projects currently using this feature.

- **Context**:

  - 2023-11-16 17:17 Email alert from Sentry notifying us that 80% of replay quota exhausted.
  - 2023-11-16 18:01 Email alert from Sentry notifying us that 100% of replay quota exhausted. No more quota until monthly reset on 14th December.
  - 2023-11-17 09:21 Operations Engineering Team aware of email alert from Sentry.
  - 2023-11-17 10:38 Investigation started. Data shows that spike as a result of replays from one project.
  - 2023-11-17 10:43 First contact with the Service Team to alert them to issues and to establish what may have changed. A change was made to the config that enabled this feature for their app. The config resulted in the spike. Agreed remediation work (i.e. to remove the trigger on non-error transactions) to reduce risk of recurrence.
  - 2023-11-17 12:21 Search of Github org to identify any other impacted teams. Two other teams identified, but not contributed to replay sessions. Teams contacted to notify them that the quota is exhausted. No immediate impact to teams.
  - 2023-11-17 14:00 Contacted Sentry Customer Success Manager to discuss estimations for a potential quota increase, plus some user questions about feature behaviour to help set appropriate limits.
  - 2023-11-17 14:40 PR raised to remove triggers for % transactions.
  - 2023-11-17 15:40 PR approved
  - 2023-11-17 15:45 PR merged

- **Resolution**: Worked with Service Team to update configuration to reduce risk of further quota spikes. It is likely that until the quota is increased that further breaches may occur.

- **Review Actions**:
  - Improve detection of spikes by adding Replays to existing anolmoly detection and alerting - **TODO**
  - Forward automated email alerts from Sentry to alerts channel in slack to improve visibility an align to operational practices - **Done**
  - Increase Replay subscription to allow users to be able to use the feature - **TODO**
  - Create user documentation to help Service Teams set appropraite sample rates - **TODO**
