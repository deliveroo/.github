## :warning: Note: This is a public repository (anyone outside Deliveroo can view it)

## Available workflow templates

- `workflow-templates/jira-report-to-slack.yml`
  - Automates Jira reporting into Slack.
  - Queries Jira with JQL and posts a summary into Slack on a schedule or manual trigger.
  - Configure these repository settings before enabling:
    - **Repository Variables**
      - `JIRA_BASE_URL` (for example, `https://your-domain.atlassian.net`)
      - `JIRA_REPORT_JQL` (for example, `project = ENG AND statusCategory != Done ORDER BY priority DESC, updated DESC`)
      - `JIRA_REPORT_MAX_RESULTS` (optional, default is `25`, max is `100`)
    - **Repository Secrets**
      - `JIRA_USER_EMAIL`
      - `JIRA_API_TOKEN`
      - `SLACK_WEBHOOK_URL`
