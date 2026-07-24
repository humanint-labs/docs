# Source: https://capisum.com/

# One API for payments,wallets, crypto, and accounts.

Connect payment gateways, digital banks, crypto platforms, and account infrastructure providers through one standard API.

[Get started](https://capisum.com/waitlist) [View docs](https://capisum.com/docs)

Live flow

pay-inpayoutaccount

Your app sends request

POST /v1/transactions

Capisum receives and normalizes request

✓ Capisum validates amount, currency, customer, and provider

Capisum routes to selected provider

→ provider: paystack

Provider processes transaction

✓ Paystack confirms pay-in

Capisum returns one standard response

200 OK

{

"status": "successful",

"provider": "paystack",

"reference": "cap\_txn\_9x82k"

}

Trusted by engineering teams

- stripe
- flutterwave
- plaid
- paystack
- railway
- shopify

Product

## What's in Capisum?

Everything you need to integrate and manage fragmented fintech providers through one API.

- ### Unified API objects
 
 Work with one transaction, customer, and account model across every provider—same fields, same lifecycle.
 
- ### Provider adapters
 
 Each gateway, bank, PSP, and crypto platform sits behind an adapter that maps your request to its native API.
 
- ### Manual provider selection
 
 Choose the provider per transaction in the MVP—predictable routing you control before optional smart routing ships.
 
- ### Standard errors
 
 A consistent error shape with stable codes, so handling and retries work the same everywhere.
 
- ### Standard responses
 
 Normalized responses regardless of which provider executed the transaction.
 
- ### Developer-ready surface
 
 One request shape, clear docs, and a REST API built for engineers shipping real volume.
 
- ### Multi-category providers
 
 Payment gateways, digital banks, crypto ramps, and account infrastructure through one integration layer.
 
- ### Future smart routing
 
 Smart routing and failover are planned as an optional dashboard feature—never automatic in the MVP.
 

Foundation

## Built on a foundation of standardization

Capisum is designed for teams who need one dependable abstraction over changing provider APIs.

- ### Unified objects
 
 Transactions, customers, accounts, and providers share one schema—your app reads the same regardless of backend.
 
- ### Adapter layer
 
 Provider-specific translation happens behind adapters so your integration surface stays stable.
 
- ### Consistent errors
 
 Stable error codes and envelopes mean observability, retries, and support playbooks work once.
 

## One API, many providers

Connect payment gateways, digital banks, crypto platforms, and account infrastructure through a single integration layer.

- Live
 
 ### Paystack
 
 Accept cards, bank transfers, and local payment methods.
 
 Payment gateway
 
 Pay-inPayout
 
- Live
 
 ### Flutterwave
 
 Process payments across cards, transfers, and mobile money.
 
 Payment gateway
 
 Pay-inPayout
 
- Live
 
 ### Monnify
 
 Collect payments through virtual accounts and bank transfers.
 
 Payment gateway
 
 Pay-inAccounts
 
- Beta
 
 ### Interswitch
 
 Route card and switch-based payment transactions.
 
 Payment gateway
 
 Pay-inRouting
 
- Beta
 
 ### Remita
 
 Handle government and enterprise payment collections.
 
 Payment gateway
 
 Pay-inPayout
 
- Beta
 
 ### Korapay
 
 Accept cards, bank transfers, and checkout payments.
 
 Payment gateway
 
 Pay-inPayout
 
- Beta
 
 ### SeerBit
 
 Process multi-channel payment collections and disbursements.
 
 Payment gateway
 
 Pay-inPayout
 
- Beta
 
 ### Squad
 
 Run card, transfer, and virtual account payment flows.
 
 Payment gateway
 
 Pay-inAccounts
 

[Show more providers](https://capisum.com/providers)

## Simple monthly pricing

Start free with usage units, then subscribe monthly as you grow. No annual plans. Expensive provider operations like balance checks use weighted units; retries, polling, reconciliation, and webhooks are never billed.

- Free

 ₦0

 Explore Capisum with no card required

 - 1,000 usage units / month
 - Up to 2 connected providers
 - Sandbox and production access
 - Standardized responses
 - No card required

 [Get started](https://capisum.com/waitlist)

- Recommended

 Starter

 ₦15,000/mo

 For teams shipping real fintech workflows

 - 150,000 usage units / month
 - Up to 5 connected providers
 - Pay-in, payout, and more
 - Balance checks and account resolution
 - Provider status monitoring
 - Overage at ₦100 / 1,000 units
 - Email support

 [Start building](https://capisum.com/waitlist)

- Growth

 ₦45,000/mo

 For higher volume and unlimited providers

 - 750,000 usage units / month
 - Unlimited connected providers
 - Pay-in, payout, and more
 - Provider status monitoring
 - Overage at ₦50 / 1,000 units
 - Priority email support

 [Choose Growth](https://capisum.com/waitlist)

- Enterprise

 From ₦250,000/mo

 Custom limits, SLA, and reconciliation controls

 - Custom usage limits
 - Unlimited connected providers
 - Higher rate limits
 - Priority support
 - SLA
 - Custom reconciliation controls

 [Contact us](https://capisum.com/contact)


## Questions, answered.

Everything you need to know about building with Capisum.

### What is Capisum?

Capisum is a unified API layer that lets your app connect to payment gateways, digital banks, wallets, crypto platforms, and account infrastructure providers through one standard integration.

### How does Capisum pricing work?

Capisum uses monthly subscription plans billed in NGN: Free (₦0, 1,000 usage units, 2 providers), Starter (₦15,000/mo, 150,000 units, 5 providers), Growth (₦45,000/mo, 750,000 units, unlimited providers), and Enterprise (from ₦250,000/mo with custom limits). There is no annual billing. Standard API requests use 1 usage unit; balance checks and account resolution use weighted units. Internal retries, polling, reconciliation, and webhook processing are never billed.

### Does Capisum process payments directly?

No. Capisum does not replace the underlying providers. It standardizes how your application connects to them, sends requests, receives responses, and handles provider differences.

### Which providers can I connect to?

Capisum is designed to support providers like Paystack, Flutterwave, Monnify, OPay, PalmPay, Kuda, Quidax, Binance, Luno, Bridge, Unit, Treasury Prime, and more.

### Can I choose which provider handles a transaction?

Yes. In the MVP, your app can manually select the provider for each transaction. Smart routing can be added later as an optional feature.

[View all questions](https://capisum.com/faq)

Get started

## Get started in seconds

Join the waitlist for early access or read the API docs to explore the unified request and response shapes.

- [**Join the waitlist**\\ \\ Get early access to the unified API, dashboard, and provider adapters as they roll out.\\ \\ Join waitlist](https://capisum.com/waitlist)
- [**Read the API docs**\\ \\ Explore endpoints, standard objects, and example requests before you integrate.\\ \\ View docs](https://capisum.com/docs)