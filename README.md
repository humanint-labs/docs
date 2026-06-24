# Capisum documentation

Mintlify documentation for the Capisum public integrator API (`/v1/*`).

## Local preview

```bash
npm i -g mint
cd docs
mint dev
```

Open `http://localhost:3000`.

## Validate before publishing

```bash
mint validate
mint broken-links
mint a11y
```

## Regenerate API reference

The OpenAPI spec is generated from shipped public routes in `capisum-api`:

```bash
python3 ../capisum-api/scripts/generate-public-openapi.py
```

This writes `openapi.json` and `../capisum-api/docs/api/public-openapi.json`. Mintlify generates endpoint pages from `openapi.json` via `docs.json` navigation.

## What this site covers

- Customer API authentication, payouts, and transactions
- OpenAPI reference with interactive playground

Dashboard, admin, and provider credential APIs are documented only in product UI — not in this site.

## Publishing

Push to the default branch. Mintlify deploys automatically when the GitHub app is connected.
