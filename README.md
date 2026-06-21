# Numeral (numeral)

Numeral (Numeral HQ) is a sales-tax compliance and automation platform for ecommerce and SaaS companies. Its REST API calculates real-time sales tax by customer location at state, county, city, and district granularity, records transactions and refunds, and manages products and customers, while the broader platform handles registrations, nexus monitoring, filing, and remittance. Not to be confused with Numeral (numeral.io), an unrelated payment-operations company now part of Mambu.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/apis.yml)

## Tags

- Sales Tax
- Tax Compliance
- Tax Calculation
- Ecommerce
- SaaS

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Numeral Tax Calculations API

Calculates real-time sales tax for a given product, customer, and address or IP at state, county, city, and district granularity, returning per-line-item and total tax amounts. Includes platform/marketplace calculations.

- **Human URL:** [https://docs.numeral.com/api-reference/introduction](https://docs.numeral.com/api-reference/introduction)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Tax Calculation
- Sales Tax
- Rates

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/introduction)
- [API Reference](https://docs.numeral.com/api-reference/v2026-03-01/endpoint/calculations)
- [OpenAPI](openapi/numeral-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/numeral.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/numeral.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Numeral Transactions API

Records completed sales against a prior calculation, retrieves and deletes transactions, and manages refunds and refund reversals that feed downstream filing and remittance.

- **Human URL:** [https://docs.numeral.com/api-reference/v2026-03-01/endpoint/transactions](https://docs.numeral.com/api-reference/v2026-03-01/endpoint/transactions)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Transactions
- Sales
- Refunds

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/v2026-03-01/endpoint/transactions)
- [OpenAPI](openapi/numeral-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/numeral.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/numeral.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Numeral Filings API

Sales-tax return filing and remittance (Autofile) across all US states, driven by recorded transactions. Filing and remittance are delivered as managed platform services rather than self-serve public REST endpoints; transaction data captured via the API flows into them.

- **Human URL:** [https://www.numeral.com/product/api](https://www.numeral.com/product/api)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Filings
- Remittance
- Autofile

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/introduction)
- [Plans](https://www.numeral.com/pricing)

### Numeral Registrations & Nexus API

State sales-tax registration (Autoregister) and physical/economic nexus monitoring with state-crossing alerts. Provided as managed platform services on top of API-captured transaction data rather than as self-serve public REST endpoints.

- **Human URL:** [https://www.numeral.com/product/api](https://www.numeral.com/product/api)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Registrations
- Nexus
- Monitoring

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/introduction)
- [Plans](https://www.numeral.com/pricing)

### Numeral Products & Tax Codes API

Creates, categorizes, lists, and deletes products and maps them to tax-code product categories that drive correct taxability, plus customer records with tax-exemption status.

- **Human URL:** [https://docs.numeral.com/api-reference/v2026-03-01/endpoint/products](https://docs.numeral.com/api-reference/v2026-03-01/endpoint/products)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Products
- Tax Codes
- Classification

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/v2026-03-01/endpoint/products)
- [OpenAPI](openapi/numeral-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/numeral.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/numeral.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Numeral Webhooks

Event notifications for compliance and transaction lifecycle changes (e.g., filing, registration, and nexus events). Webhook delivery is offered through the Numeral platform; no public webhook subscription endpoint is documented in the REST API reference as of this writing (see review.yml).

- **Human URL:** [https://docs.numeral.com/api-reference/introduction](https://docs.numeral.com/api-reference/introduction)
- **Base URL:** `https://api.numeralhq.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.numeral.com/api-reference/introduction)

## Common Properties

- [GitHub Organization](https://github.com/numeralhq)
- [LinkedIn](https://www.linkedin.com/company/numeralhq)
- [Website](https://www.numeral.com/)
- [Documentation](https://docs.numeral.com/api-reference/introduction)
- [Plans](plans/numeral-plans-pricing.yml)
- [Rate Limits](rate-limits/numeral-rate-limits.yml)
- [Fin Ops](finops/numeral-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
