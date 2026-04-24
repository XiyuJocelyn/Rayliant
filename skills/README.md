# Skills

This folder contains the **agent skills** — modular, reusable capabilities that the Rayliant sales management AI agent can invoke during a conversation or automated workflow.

## What Is a Skill?

A skill is a self-contained unit of logic that the agent calls to perform a specific sales-related task. Skills operate on data retrieved from the [database](../database/README.md) or via [tools](../tools/README.md) and return structured results that the agent can reason over.

## Planned Skills

| Skill | Description |
|---|---|
| `summarise_lead` | Summarise a lead's history, last activity and next recommended action |
| `draft_email` | Draft a personalised outreach or follow-up email for a prospect |
| `forecast_pipeline` | Estimate expected revenue for the current quarter based on open opportunities |
| `score_opportunity` | Assign a priority score to an open deal based on engagement and deal size |
| `generate_call_brief` | Generate a pre-call research brief for a scheduled sales call |
| `analyse_lost_deals` | Identify patterns in lost deals to surface coaching opportunities |

## Adding a New Skill

1. Create a new file (or subfolder for complex skills) inside `skills/`.
2. Implement the skill interface expected by the agent runtime.
3. Register the skill in the agent's skill registry.
4. Add tests and update this README with the new skill's description.
