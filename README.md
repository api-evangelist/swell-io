# Swell

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Swell is a customizable, API-first headless commerce platform powering modern B2C, B2B, subscription, and marketplace experiences. It exposes a server-side Backend API for managing the full commerce data model (products, variants, carts, orders, payments, refunds, shipments, returns, subscriptions, accounts, invoices, coupons, promotions, gift cards, content, files, events, webhooks) plus a public-key client-side Frontend API for storefronts and an experimental GraphQL endpoint. The platform ships official Node and PHP libraries, a universal JavaScript SDK (Swell.js), headless storefront starters for Next.js (Horizon, verswell-commerce, nextjs-commerce) and Nuxt (Origin), a Swell Apps platform with CLI and Apps SDK for extending the data and logic layers via custom data models, events, notifications, webhooks, and edge functions running in 200+ locations, plus AI coding-agent skills and Claude Code plugins.

**Areas:** Commerce · Headless Commerce · API-First · Consumer · B2B · Subscription · Marketplace · Wholesale · Storefront · Checkout · Payments · Cart

## Swell on APIs.io

Everything profiled for Swell is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/swell-io/](https://apis.io/providers/swell-io/)** — or go straight to one of the APIs or properties below.

### APIs (34)

- [Swell GraphQL API](https://apis.io/apis/swell-io/swell-graphql-api/) — Experimental (alpha) GraphQL endpoint that exposes a curated subset of the storefront commerce model — products, attributes, categories, accounts, sessions,…
- [Swell Webhooks](https://apis.io/apis/swell-io/swell-webhooks-api/) — Event-driven HTTP callbacks for cart, order, subscription, payment, account, and product lifecycle events. Configurable via the dashboard (Developer →…
- [Swell Apps Platform](https://apis.io/apis/swell-io/swell-apps-platform/) — Swell Apps extend the platform with custom data models (added fields or new entities), events (triggering functions, webhooks, and notifications), edge…
- [Swell Account Addresses API](https://apis.io/apis/swell-io/swell-io-account-addresses-api/) — Saved shipping/billing addresses on an account.
- [Swell Account API](https://apis.io/apis/swell-io/swell-io-account-api/) — Authenticated customer account operations.
- [Swell Account Cards API](https://apis.io/apis/swell-io/swell-io-account-cards-api/) — Saved payment cards on an account.
- [Swell Account Credits API](https://apis.io/apis/swell-io/swell-io-account-credits-api/) — Store credit balances and transactions per account.
- [Swell Account Session API](https://apis.io/apis/swell-io/swell-io-account-session-api/) — Login, logout, and session recovery.
- [Swell Accounts API](https://apis.io/apis/swell-io/swell-io-accounts-api/) — Customer accounts including billing/shipping, saved cards, and history.
- [Swell Attributes API](https://apis.io/apis/swell-io/swell-io-attributes-api/) — Product attributes used for filtering and faceted search.
- [Swell Cart API](https://apis.io/apis/swell-io/swell-io-cart-api/) — Session-scoped shopping cart for the current visitor.
- [Swell Carts API](https://apis.io/apis/swell-io/swell-io-carts-api/) — Pending purchase requests that can be converted into orders.
- [Swell Categories API](https://apis.io/apis/swell-io/swell-io-categories-api/) — Category tree and product taxonomy.
- [Swell Checkout API](https://apis.io/apis/swell-io/swell-io-checkout-api/) — Cart conversion and order placement.
- [Swell Content API](https://apis.io/apis/swell-io/swell-io-content-api/) — Pages, custom data models, and stored records.
- [Swell Coupons API](https://apis.io/apis/swell-io/swell-io-coupons-api/) — Coupon definitions with codes, redemptions, and discount rules.
- [Swell Events API](https://apis.io/apis/swell-io/swell-io-events-api/) — Event records emitted by the platform.
- [Swell Files API](https://apis.io/apis/swell-io/swell-io-files-api/) — Stored files (images, attachments) served via Swell CDN.
- [Swell Gift Cards API](https://apis.io/apis/swell-io/swell-io-gift-cards-api/) — Gift cards, debit transactions, and gift card products.
- [Swell Invoices API](https://apis.io/apis/swell-io/swell-io-invoices-api/) — Invoices generated for subscription billing cycles and B2B orders.
- [Swell Orders API](https://apis.io/apis/swell-io/swell-io-orders-api/) — Customer orders, line items, financial totals, and lifecycle.
- [Swell Payments API](https://apis.io/apis/swell-io/swell-io-payments-api/) — Payment transactions, refunds, and gateway settlement.
- [Swell Products API](https://apis.io/apis/swell-io/swell-io-products-api/) — Product catalog including variants, options, bundles, gift cards, and subscription products.
- [Swell Promotions API](https://apis.io/apis/swell-io/swell-io-promotions-api/) — Automatic promotion rules applied at cart and checkout.
- [Swell Purchase Links API](https://apis.io/apis/swell-io/swell-io-purchase-links-api/) — Shareable purchase links that prefill a cart.
- [Swell Refunds API](https://apis.io/apis/swell-io/swell-io-refunds-api/) — Refund records linked to a payment.
- [Swell Returns API](https://apis.io/apis/swell-io/swell-io-returns-api/) — Customer return merchandise authorizations.
- [Swell Shipments API](https://apis.io/apis/swell-io/swell-io-shipments-api/) — Fulfillment shipments, tracking, and split fulfillment.
- [Swell Stock API](https://apis.io/apis/swell-io/swell-io-stock-api/) — Stock levels and stock adjustments across locations.
- [Swell Store API](https://apis.io/apis/swell-io/swell-io-store-api/) — Public store settings, currencies, payment settings, and menus.
- [Swell Subscription Plans API](https://apis.io/apis/swell-io/swell-io-subscription-plans-api/) — Plan templates that define billing schedule and price for recurring products.
- [Swell Subscriptions API](https://apis.io/apis/swell-io/swell-io-subscriptions-api/) — Recurring billing subscriptions and plans.
- [Swell Variants API](https://apis.io/apis/swell-io/swell-io-variants-api/) — Variant-level inventory and pricing under a parent product.
- [Swell Webhooks API](https://apis.io/apis/swell-io/swell-io-webhooks-api/) — Webhook subscriptions for receiving event callbacks.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (13)

Multi-step workflows that chain operations into a business task.

- [Swell Create Cart and Apply Coupon](https://apis.io/arazzos/swell-io/swell-io-apply-coupon-to-cart-workflow/)
- [Swell Build Cart and Convert to Order](https://apis.io/arazzos/swell-io/swell-io-build-cart-convert-order-workflow/)
- [Swell Find and Cancel Active Subscription](https://apis.io/arazzos/swell-io/swell-io-cancel-subscription-workflow/)
- [Swell Capture and Refund Payment](https://apis.io/arazzos/swell-io/swell-io-capture-refund-payment-workflow/)
- [Swell Create Category and Product](https://apis.io/arazzos/swell-io/swell-io-categorize-product-workflow/)
- [Swell Create and Verify Product](https://apis.io/arazzos/swell-io/swell-io-create-product-workflow/)
- [Swell Create and Verify Subscription](https://apis.io/arazzos/swell-io/swell-io-create-subscription-workflow/)
- [Swell Find-or-Create Customer and Order](https://apis.io/arazzos/swell-io/swell-io-find-or-create-customer-order-workflow/)
- [Swell Onboard Customer and Place Order](https://apis.io/arazzos/swell-io/swell-io-onboard-customer-order-workflow/)
- [Swell Storefront Validate and Apply Coupon](https://apis.io/arazzos/swell-io/swell-io-storefront-apply-coupon-workflow/)
- [Swell Storefront Add Item and Submit Order](https://apis.io/arazzos/swell-io/swell-io-storefront-checkout-workflow/)
- [Swell Storefront Register and Log In](https://apis.io/arazzos/swell-io/swell-io-storefront-register-login-workflow/)
- [Swell Storefront Adjust Cart Item Quantity](https://apis.io/arazzos/swell-io/swell-io-storefront-update-cart-item-workflow/)

#### GraphQL (1)

GraphQL schemas.

- [Swell GraphQL API](https://apis.io/graphqls/swell-io/swell-io-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Swell Io Agentic Access](https://apis.io/agentic-access/swell-io/swell-io-agentic-access/)

#### JSON Schema (7)

The data models the API reads and writes.

- [Swell Account](https://apis.io/schemas/swell-io/swell-account/)
- [Swell Cart](https://apis.io/schemas/swell-io/swell-cart/)
- [Swell Order](https://apis.io/schemas/swell-io/swell-order/)
- [Swell Payment](https://apis.io/schemas/swell-io/swell-payment/)
- [Swell Product](https://apis.io/schemas/swell-io/swell-product/)
- [Swell Subscription](https://apis.io/schemas/swell-io/swell-subscription/)
- [Swell Webhook Subscription](https://apis.io/schemas/swell-io/swell-webhook/)

#### JSON Structure (4)

Data models expressed in JSON Structure.

- [Swell Account Structure](https://apis.io/json-structure/swell-io/swell-account-structure/)
- [Swell Order Structure](https://apis.io/json-structure/swell-io/swell-order-structure/)
- [Swell Product Structure](https://apis.io/json-structure/swell-io/swell-product-structure/)
- [Swell Subscription Structure](https://apis.io/json-structure/swell-io/swell-subscription-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Swell Io Context](https://apis.io/jsonld/swell-io/swell-io-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Swell Commerce Vocabulary](https://apis.io/vocabularies/swell-io/swell-io-vocabulary/)

#### Examples (6)

Example requests and responses.

- [Swell Account Create Example](https://apis.io/examples/swell-io/swell-account-create-example/)
- [Swell Cart Add Item Example](https://apis.io/examples/swell-io/swell-cart-add-item-example/)
- [Swell Order Create Example](https://apis.io/examples/swell-io/swell-order-create-example/)
- [Swell Product Create Example](https://apis.io/examples/swell-io/swell-product-create-example/)
- [Swell Subscription Create Example](https://apis.io/examples/swell-io/swell-subscription-create-example/)
- [Swell Webhook Event Example](https://apis.io/examples/swell-io/swell-webhook-event-example/)

#### Collections (35)

Postman and Open Collection request collections.

- [Swell Backend API](https://apis.io/collections/swell-io/open-swell-backend-api/)
- [Swell Frontend API](https://apis.io/collections/swell-io/open-swell-frontend-api/)
- [Swell Backend Account Addresses API](https://apis.io/collections/swell-io/open-swell-io-account-addresses-api/)
- [Swell Backend Addresses Account API](https://apis.io/collections/swell-io/open-swell-io-account-api/)
- [Swell Backend Account Addresses Account Cards API](https://apis.io/collections/swell-io/open-swell-io-account-cards-api/)
- [Swell Backend Account Addresses Account Credits API](https://apis.io/collections/swell-io/open-swell-io-account-credits-api/)
- [Swell Backend Account Addresses Account Session API](https://apis.io/collections/swell-io/open-swell-io-account-session-api/)
- [Swell Backend Account Addresses Accounts API](https://apis.io/collections/swell-io/open-swell-io-accounts-api/)
- [Swell Backend Account Addresses Attributes API](https://apis.io/collections/swell-io/open-swell-io-attributes-api/)
- [Swell Backend Account Addresses Cart API](https://apis.io/collections/swell-io/open-swell-io-cart-api/)
- [Swell Backend Account Addresses Carts API](https://apis.io/collections/swell-io/open-swell-io-carts-api/)
- [Swell Backend Account Addresses Categories API](https://apis.io/collections/swell-io/open-swell-io-categories-api/)
- [Swell Backend Account Addresses Checkout API](https://apis.io/collections/swell-io/open-swell-io-checkout-api/)
- [Swell Backend Account Addresses Content API](https://apis.io/collections/swell-io/open-swell-io-content-api/)
- [Swell Backend Account Addresses Coupons API](https://apis.io/collections/swell-io/open-swell-io-coupons-api/)
- [Swell Backend Account Addresses Events API](https://apis.io/collections/swell-io/open-swell-io-events-api/)
- [Swell Backend Account Addresses Files API](https://apis.io/collections/swell-io/open-swell-io-files-api/)
- [Swell Backend Account Addresses Gift Cards API](https://apis.io/collections/swell-io/open-swell-io-gift-cards-api/)
- [Swell Backend Account Addresses Invoices API](https://apis.io/collections/swell-io/open-swell-io-invoices-api/)
- [Swell Backend Account Addresses Orders API](https://apis.io/collections/swell-io/open-swell-io-orders-api/)
- [Swell Backend Account Addresses Payments API](https://apis.io/collections/swell-io/open-swell-io-payments-api/)
- [Swell Backend Account Addresses Products API](https://apis.io/collections/swell-io/open-swell-io-products-api/)
- [Swell Backend Account Addresses Promotions API](https://apis.io/collections/swell-io/open-swell-io-promotions-api/)
- [Swell Backend Account Addresses Purchase Links API](https://apis.io/collections/swell-io/open-swell-io-purchase-links-api/)
- [Swell Backend Account Addresses Refunds API](https://apis.io/collections/swell-io/open-swell-io-refunds-api/)
- …and 10 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Swell — jsonschema rules](https://apis.io/rules/swell-io/swell-io-jsonschema-spectral-rules/)
- [Swell — swell rules](https://apis.io/rules/swell-io/swell-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Swell Io Authentication](https://apis.io/security/swell-io/swell-io-authentication/)
- [Swell Io Domain Security](https://apis.io/security/swell-io/swell-io-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Swell Io Plans Pricing](https://apis.io/plans/swell-io/swell-io-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Swell Io Rate Limits](https://apis.io/rate-limits/swell-io/swell-io-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Swell Io Finops](https://apis.io/finops/swell-io/swell-io-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.swell.is/)
- [Documentation](https://developers.swell.is)
- [Getting started](https://developers.swell.is/guides/quickstart-guide)
- [Pricing](https://www.swell.is/pricing)
- [Support](https://www.swell.is/help)
- [Changelog](https://www.swell.is/changelog)
- [Blog](https://www.swell.is/blog)
- [Terms of service](https://www.swell.is/legal/terms-of-service)
- [Privacy policy](https://www.swell.is/legal/privacy-policy)
- [GitHub](https://github.com/swellstores)
- [Status](https://status.swell.store/)

## API Evangelist rating

**Kin Score 56.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 62.3 |
| Contract governance | 27.3 |
| Operational transparency | 42.1 |
| Developer ergonomics | 82.1 |
| Access clarity | 52.6 |

**Agent readiness 20.8** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly (partial credit) |

**Regulatory alignment 22.3** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/swell-io/](https://apis.io/providers/swell-io/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Swell: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/swell-io/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
