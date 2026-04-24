# Database

This folder contains everything related to the **persistent data storage** for the Rayliant sales management AI agent — schemas, migrations, seed data and query helpers.

## Purpose

The database layer is the single source of truth for all sales data the agent reads from and writes to, including contacts, accounts, opportunities, activities and agent memory/state.

## Planned Contents

| Item | Description |
|---|---|
| `schema/` | Table and collection definitions (SQL DDL or ORM models) |
| `migrations/` | Versioned schema migration scripts |
| `seeds/` | Sample/demo data for development and testing |
| `queries/` | Reusable query helpers and stored procedures |
| `config/` | Database connection configuration templates |

## Key Entities

| Entity | Description |
|---|---|
| `contacts` | Individual people the sales team is engaging with |
| `accounts` | Companies or organisations associated with contacts |
| `opportunities` | Open deals tracked through the sales pipeline |
| `activities` | Logged interactions: calls, emails, meetings, notes |
| `agent_memory` | Persisted agent context, session state and learned preferences |

## Getting Started

1. Copy `config/database.example.env` to `config/database.env` and fill in your connection details.
2. Run the migration scripts in `migrations/` in order to set up the schema.
3. Optionally run the seed scripts in `seeds/` to populate demo data.
