---
owner_slack: "#operations-engineering-alerts"
title: Incident Log
last_reviewed_on: 2023-11-21
review_in: 3 months
---

# Incident Log

This is a log of Operations Engineering managed incidents.

## Q4 2023 (October to Decmeber)

- **Mean Time to Repair**: 6h 24m

- **Mean Time to Resolve**: TBC

### Incident on 2023-11-17 - Sentry Session Replay Quota Breach

- **Key events**
  - First detected: 2023-11-16 09:21
  - Repaired: 2023-11-16 15:45
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
