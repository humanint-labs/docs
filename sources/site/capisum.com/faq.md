# Source: https://capisum.com/faq

# Questions, answered.

Everything you need to know about building with Capisum.

### What is Capisum?

Capisum is a unified API layer that lets your app connect to payment gateways, digital banks, wallets, crypto platforms, and account infrastructure providers through one standard integration.

### Does Capisum process payments directly?

No. Capisum does not replace the underlying providers. It standardizes how your application connects to them, sends requests, receives responses, and handles provider differences.

### Which providers can I connect to?

Capisum is designed to support providers like Paystack, Flutterwave, Monnify, OPay, PalmPay, Kuda, Quidax, Binance, Luno, Bridge, Unit, Treasury Prime, and more.

### Can I choose which provider handles a transaction?

Yes. In the MVP, your app can manually select the provider for each transaction. Smart routing can be added later as an optional feature.

### What operations will Capisum support?

The initial focus is pay-ins, payouts, provider selection, transaction status, standardized responses, and provider monitoring.

### Does Capisum handle KYC or compliance?

No. For now, customers still complete KYC, KYB, and compliance directly with the underlying provider. Capisum focuses on integration, standardization, routing, and observability.

### Do I need separate accounts with each provider?

Yes. You will need active provider accounts and credentials for the providers you want to use. Capisum helps you connect and operate them through one API.

### What happens when a provider fails?

Capisum returns a standardized error format so your app can handle failures consistently. Later, smart routing can automatically retry or switch providers based on your configuration.

### Is Capisum for developers?

Yes. Capisum is built for engineering teams that need one clean API instead of maintaining multiple provider integrations.

### Is there a sandbox?

Yes. The platform should include a sandbox mode so teams can test integrations before going live.