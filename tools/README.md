# Tools

This folder contains the **agent tools** — integrations and utility wrappers that allow the Rayliant AI agent to interact with external systems and services.

## What Is a Tool?

A tool is an interface between the agent and a third-party service or internal utility. The agent calls tools when it needs to read from or write to an external system (e.g. fetching a contact from the CRM, sending an email, or looking up calendar availability).

## Planned Tools

| Tool | Description |
|---|---|
| `crm_client` | Read and write contacts, accounts, and opportunities in the CRM (e.g. Salesforce, HubSpot) |
| `email_sender` | Send emails via an SMTP gateway or email API (e.g. SendGrid, Mailgun) |
| `calendar_client` | Query and create calendar events for scheduling sales calls |
| `web_search` | Search the web for prospect research and company news |
| `document_parser` | Extract structured data from uploaded sales documents or attachments |
| `notification_sender` | Push notifications to Slack or Microsoft Teams channels |

## Adding a New Tool

1. Create a new file (or subfolder for complex integrations) inside `tools/`.
2. Implement the tool interface expected by the agent runtime.
3. Add required credentials or configuration to the environment variable documentation.
4. Register the tool with the agent and update this README.
