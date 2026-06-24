# Source: https://capisum.com/products

# Infrastructure for fintech integrations.

Capisum gives your team one API layer for providers, routing, logs, responses, errors, and operational visibility.

[Get started](https://capisum.com/waitlist) [View docs](https://capisum.com/docs)

integration-flow.capisum

Your App

\->

Capisum

\->

Providers

POST /v1/payments

```
{
  "amount": 500000,
  "provider": "paystack",
  "currency": "NGN"
}
```

Request

12ms

Route

Paystack

Status

Settled

Unified API

## One integration surface for every provider category.

Connect payment gateways, digital wallets, banks, crypto platforms, and account infrastructure through a single API. Your app speaks Capisum — Capisum handles provider-specific details behind the scenes.

- One transaction model across gateways, wallets, crypto, and account infra
- Shared authentication and request patterns for every adapter
- Add providers without rewriting your core payment flows

unified-api.ts

capisum.payments.create({

provider: "flutterwave",

amount: 250000,

currency: "NGN",

});

Supported categories

- → Payment gateways
- → Digital banks & wallets
- → Crypto platforms
- → Account infrastructure

Provider Routing

## Choose the provider for each transaction.

Select which provider handles a payment, payout, or account operation from your dashboard. Manual routing gives you predictable control today — with room for smart routing policies as your volume grows.

- Explicit provider selection per transaction in the MVP
- Same API call shape regardless of which backend executes
- Architecture ready for future routing rules and fallbacks

routing.dashboard

Active route

Paystack · NGN pay-in

- PaystackSelected
- FlutterwaveAvailable
- MonnifyAvailable

Smart routing policies — coming later

Transaction Logs

## Full visibility into every API and provider call.

Search and inspect logs for API requests, provider calls, statuses, retries, and failures. Debug integration issues without digging through scattered provider dashboards.

- Timeline of requests, responses, and provider handoffs
- Filter by status, provider, operation, and time range
- Retry context and failure details in one searchable view

transaction-logs

| Time | Provider | Status | Latency |
| --- | --- | --- | --- |
| 14:02:11 | Paystack | settled | 142ms |
| 14:01:58 | Flutterwave | pending | 89ms |
| 14:01:42 | Kuda | failed | 210ms |
| 14:01:19 | Quidax | settled | 118ms |

Standardized Responses

## One response shape across all providers.

Every provider returns data in its own format. Capisum normalizes payloads so your application receives consistent fields, statuses, and lifecycle events — no matter which adapter ran the operation.

- Predictable response fields for payments, payouts, and accounts
- Unified status vocabulary across provider categories
- Less conditional parsing logic in your application code

response.normalized.json

```
{
  "id": "txn_8f2k9m",
  "status": "settled",
  "amount": 500000,
  "provider": "paystack",
  "provider_ref": "PSK-9281"
}
```

Same fields whether Paystack, Flutterwave, or Kuda executed the call.

Error Normalization

## Consistent errors instead of provider-specific chaos.

Map fragmented provider error messages into stable codes and envelopes. Your retry logic, observability, and support playbooks work once — not once per integration.

- Stable error codes across every supported provider
- Structured error envelopes for logging and alerting
- Clear distinction between retryable and terminal failures

errors.normalized

- INSUFFICIENT\_FUNDSterminal
 
 Normalized across any providers
 
- PROVIDER\_TIMEOUTretryable
 
 Normalized across any providers
 
- INVALID\_ACCOUNTterminal
 
 Normalized across any providers
 

Dashboard

## Your control center for integration operations.

Manage provider connections, review transactions, monitor health, and coordinate team access from one operational surface built for engineers and ops.

- Provider connection status and credential management
- Transaction monitoring with filters and detail views
- Team access controls for staging and production environments

dashboard.capisum

Transactions

12,847

Providers

8 active

Success rate

99.2%

Open issues

3

Recent activity

- Paystack adapter · credential rotated
- Flutterwave · 3 retries resolved
- Team · ops@capisum invited