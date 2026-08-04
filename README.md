# Orb (orb-billing)

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

Orb is a usage-based billing and metering platform that turns product usage events into subscriptions, prices, invoices, and credits. The Orb REST API ingests metered events, models customers, plans, prices, and items, runs subscriptions, and automates invoicing, credit ledgers, alerts, and webhooks for modern revenue teams.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/apis.yml)

## Tags

- Billing
- Usage-Based Billing
- Metering
- Subscriptions
- Invoicing
- FinOps

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Orb Customers API

Create, fetch, update, list, and delete customers by Orb ID or external ID, manage balance transactions, costs, payment methods, and hosted portal sessions.

- **Human URL:** [https://docs.withorb.com/api-reference/customer](https://docs.withorb.com/api-reference/customer)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Customers
- Accounts
- Portal

#### Properties

- [Documentation](https://docs.withorb.com/core-concepts/customers)
- [API Reference](https://docs.withorb.com/api-reference/customer)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Plans API

Define and version plans that bundle prices, with create, fetch, list, update, version, and migration operations addressable by Orb ID or external plan ID.

- **Human URL:** [https://docs.withorb.com/api-reference/plan](https://docs.withorb.com/api-reference/plan)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Plans
- Pricing
- Versions

#### Properties

- [Documentation](https://docs.withorb.com/core-concepts/plans-and-prices)
- [API Reference](https://docs.withorb.com/api-reference/plan)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Subscriptions API

Create, fetch, list, update, and cancel subscriptions, schedule and unschedule plan changes, redeem coupons, adjust price intervals and quantities, and read subscription usage, costs, and schedules.

- **Human URL:** [https://docs.withorb.com/api-reference/subscription](https://docs.withorb.com/api-reference/subscription)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Subscriptions
- Lifecycle
- Schedules

#### Properties

- [Documentation](https://docs.withorb.com/core-concepts/subscriptions)
- [API Reference](https://docs.withorb.com/api-reference/subscription)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Events & Ingestion API

Ingest timestamped, idempotent usage events into Orb's metering pipeline, then amend, deprecate, search, backfill, and inspect event volume that feeds billable metrics.

- **Human URL:** [https://docs.withorb.com/api-reference/event](https://docs.withorb.com/api-reference/event)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Events
- Ingestion
- Metering

#### Properties

- [Documentation](https://docs.withorb.com/events-and-metrics/event-ingestion)
- [API Reference](https://docs.withorb.com/api-reference/event)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Metrics API

Create, fetch, list, and update billable metrics that aggregate raw events into quantities prices can charge against.

- **Human URL:** [https://docs.withorb.com/api-reference/metrics](https://docs.withorb.com/api-reference/metrics)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Metrics
- Billable Metrics
- Usage

#### Properties

- [Documentation](https://docs.withorb.com/events-and-metrics/metrics)
- [API Reference](https://docs.withorb.com/api-reference/metrics)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Invoices API

Create one-off invoices, manage line items, fetch upcoming and issued invoices, issue, pay, mark as paid, void, and regenerate invoice and receipt PDFs.

- **Human URL:** [https://docs.withorb.com/api-reference/invoice](https://docs.withorb.com/api-reference/invoice)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Invoices
- Billing
- Line Items

#### Properties

- [Documentation](https://docs.withorb.com/invoicing/structure)
- [API Reference](https://docs.withorb.com/api-reference/invoice)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Credits & Ledger API

Track and adjust customer credit balances through ledger entries, top-ups, credit blocks, and credit notes, addressable by Orb ID or external customer ID.

- **Human URL:** [https://docs.withorb.com/api-reference/credit](https://docs.withorb.com/api-reference/credit)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Credits
- Ledger
- Prepaid

#### Properties

- [Documentation](https://docs.withorb.com/product-catalog/prepaid-credits)
- [API Reference](https://docs.withorb.com/api-reference/credit)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Prices & Items API

Define unit, tiered, package, matrix, and other price models, evaluate prices against events, and manage the items that prices and invoice line items reference.

- **Human URL:** [https://docs.withorb.com/api-reference/price](https://docs.withorb.com/api-reference/price)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Prices
- Items
- Catalog

#### Properties

- [Documentation](https://docs.withorb.com/core-concepts/plans-and-prices)
- [API Reference](https://docs.withorb.com/api-reference/price)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Alerts & Coupons API

Configure usage, cost, and credit-balance alerts on customers and subscriptions, and create, fetch, list, and archive coupons that grant discounts on subscriptions.

- **Human URL:** [https://docs.withorb.com/api-reference/alert](https://docs.withorb.com/api-reference/alert)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Alerts
- Coupons
- Discounts

#### Properties

- [Documentation](https://docs.withorb.com/guides/product-catalog/coupons)
- [API Reference](https://docs.withorb.com/api-reference/alert)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/orb-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Orb Webhooks API

At-least-once outbound webhooks for customer, subscription, invoice, credit note, and alert lifecycle events, signed with an HMAC-SHA256 X-Orb-Signature header and X-Orb-Timestamp for replay protection.

- **Human URL:** [https://docs.withorb.com/guides/integrations-and-exports/webhooks](https://docs.withorb.com/guides/integrations-and-exports/webhooks)
- **Base URL:** `https://api.withorb.com/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.withorb.com/guides/integrations-and-exports/webhooks)
- [OpenAPI](openapi/orb-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/orbcorp)
- [LinkedIn](https://www.linkedin.com/company/withorb)
- [Website](https://www.withorb.com)
- [Documentation](https://docs.withorb.com)
- [Plans](plans/orb-billing-plans-pricing.yml)
- [Rate Limits](rate-limits/orb-billing-rate-limits.yml)
- [Fin Ops](finops/orb-billing-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
