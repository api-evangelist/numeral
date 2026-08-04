# Numeral (numeral)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
