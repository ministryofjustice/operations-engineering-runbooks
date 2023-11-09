---
owner_slack: "#operations-engineering-alerts"
title: Managing RSS Feed Subscriptions in Slack
last_reviewed_on: 2023-11-09
review_in: 3 months
---

# Managing RSS Feed Subscriptions in Slack

### Adding a New RSS Feed Subscription

**Purpose**: To subscribe to a new RSS feed in the #operations-engineering-rss Slack channel.

**When to Use**: When a new relevant GitHub information source has been identified and needs to be added to the channel.

**Procedure**:

1. **Identify the RSS Feed URL**: Ensure the URL is correct and active by testing it in an RSS reader or browser.

2. **Open Slack**: Go to the `#operations-engineering-rss` channel in your Slack workspace.

3. **Use the Subscribe Command**: In the message input box, type `/feed subscribe <url>` replacing `<url>` with the actual RSS feed URL.

4. **Confirm Subscription**: Wait for Slack to confirm the subscription has been added. Verify by checking for a success message from the Slackbot or the feed integration bot.

5. **Document the Subscription**: Record the subscription in the team's feed management documentation with the URL and the date added.

#### Removing an RSS Feed Subscription

**Purpose**: To remove an existing RSS feed subscription from the #operations-engineering-rss Slack channel.

**When to Use**: When an RSS feed is no longer relevant or required, or if the feed is producing too much noise.

**Procedure**:

1. **Identify the Feed ID**: Locate the ID of the feed you wish to remove. This can be found in the channel's feed list or your team's feed management documentation e.g. `/feed list`.

2. **Open Slack**: Navigate to the `#operations-engineering-rss` channel in your Slack workspace.

3. **Use the Remove Command**: In the message input box, type `/feed remove <id>` replacing `<id>` with the actual feed ID.

4. **Confirm Removal**: Wait for Slack to confirm the feed has been removed. Confirm by looking for a success message from the Slackbot or the feed integration bot.

5. **Update Documentation**: Amend the team's feed management documentation to reflect the removal with the date it was removed.
