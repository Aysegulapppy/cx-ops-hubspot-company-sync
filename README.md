# CX Ops Lab — HubSpot Company Sync

A portfolio project that extracts company records from HubSpot, transforms the API response in n8n, and upserts the data into PostgreSQL.

## Architecture

```text
HubSpot CRM API → n8n HTTP Request → JavaScript transformation → PostgreSQL upsert
```

## What this project demonstrates

- HubSpot CRM API integration with n8n
- JSON transformation with JavaScript
- PostgreSQL loading and duplicate-safe upserts
- Sync timestamp tracking
- Local PostgreSQL with Docker

## Tech stack

HubSpot CRM API, n8n, PostgreSQL 16, Docker, JavaScript, SQL

## Setup

1. Start PostgreSQL with Docker.
2. Run `sql/create_table.sql`.
3. Import `workflows/hubspot-company-sync.template.json` into n8n.
4. Select your own HubSpot and PostgreSQL credentials.
5. Execute the workflow.

## Security

Never commit HubSpot tokens, database passwords, n8n credentials, `.env`, or real customer data.

## CV bullet

> Built a HubSpot-to-PostgreSQL CRM data pipeline using n8n, JavaScript, SQL, and Docker, including API extraction, JSON transformation, duplicate-safe upsert logic, and synchronization tracking.
