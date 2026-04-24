# Rayliant — Sales Management AI Agent

Rayliant is a company sales management AI agent designed to assist sales teams with lead tracking, pipeline management, customer insights, and automated reporting.

## Repository Structure

| Folder | Purpose |
|---|---|
| [`skills/`](./skills/README.md) | Agent skills — reusable capabilities the agent can invoke (e.g. summarise leads, draft emails, forecast pipeline) |
| [`tools/`](./tools/README.md) | Tools — integrations and utilities the agent uses to interact with external systems (e.g. CRM APIs, email, calendar) |
| [`database/`](./database/README.md) | Database — schemas, migrations, seed data and query helpers for the agent's persistent data store |
| [`workspace/`](./workspace/README.md) | Workspace — scratch space for agent reasoning, session state, generated artefacts and logs |

## Getting Started

1. Clone the repository.
2. Review the README in each folder to understand its role.
3. Configure your environment variables and database connection (see [`database/`](./database/README.md)).
4. Register your external service credentials under [`tools/`](./tools/README.md).
5. Launch the agent and start managing your sales pipeline.