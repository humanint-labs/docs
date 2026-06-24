# Capisum documentation

## About this project

- Mintlify docs for the **Capisum customer API** (`/v1/*`)
- Pages are MDX with YAML frontmatter; navigation in `docs.json`
- OpenAPI spec: `openapi.json` (customer endpoints only)

## Terminology

- **Customer API** — `/v1/*`, API key auth (`cps_...`)
- **Dashboard API** — `/api/v1/*`, JWT auth — do not document here
- **Minor units** — smallest currency unit (kobo, pesewa, cent)
- **Catalog vs connected** — `GET /v1/providers` lists available slugs, not connection status

## Style

- Second person, active voice, sentence case headings
- Root-relative internal links without file extensions (`/quickstart`)
- Document only what API consumers can call on `/v1/*`

## Content boundaries

**Document:** authentication, payouts, transactions, pagination, idempotency, errors.

**Do not document:** dashboard session APIs, API key CRUD, provider credential management, routing CRUD, billing, audit, team, stats, incoming webhooks, Capisum admin `/api/v1/internal/*`.

## Source of truth

Implementation: `../capisum-api/src/app.ts` (public routes under `/v1`).
Postman customer folder: `../capisum-api/docs/api/postman-collection.json`.
