
# Method based on a reply from Gemini to the prompt "how can i integrate slack to databricks? "

 How you integrate Slack with Databricks depends entirely on what you are trying to achieve. The three most common use cases include receiving automated alerts/dashboards, using AI agents to interact with Slack, or pulling Slack data into Databricks for analysis.

Here is how you can set up each scenario:

---

## 1. Native Slack Notifications (Dashboards & Alerts)

If your goal is to have Databricks automatically send a visual snapshot of AI/BI Dashboards or job status alerts directly into a Slack channel, you can use Databricks' native **Notification Destinations**.

### Step 1: Create a Slack App

1. Go to the [Slack API console](https://www.google.com/search?q=https://api.slack.com/apps) and click **Create an App** (from scratch).
2. Under **Features > OAuth & Permissions**, scroll to **Scopes** and add these Bot Token Scopes:
* `incoming-webhook`
* `files:write` (required to post PDF attachments/snapshots)
* `files:read`
* `chat:write`


3. Click **Install to Workspace**, choose your target channel, and authorize it.
4. Copy the **Bot User OAuth Token** and the **Webhook URL**. Also, grab your Slack **Channel ID** from the channel's details page in Slack.

### Step 2: Connect it in Databricks

1. Log into Databricks as a workspace admin.
2. Go to **Settings > Workspace admin > Notifications** (or Notification destinations).
3. Click **Add destination** and select **Slack**.
4. Paste your Webhook URL, OAuth Token, and Channel ID.

Once saved, any user with edit permissions on a dashboard or job can add this Slack destination as a subscriber.

---

