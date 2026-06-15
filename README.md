# Swell (swell-io)

Swell is a customizable, API-first headless commerce platform powering modern B2C, B2B, subscription, and marketplace experiences. It exposes a server-side Backend API for managing the full commerce data model (products, variants, carts, orders, payments, refunds, shipments, returns, subscriptions, accounts, invoices, coupons, promotions, gift cards, content, files, events, webhooks) plus a public-key client-side Frontend API for storefronts and an experimental GraphQL endpoint. The platform ships official Node and PHP libraries, a universal JavaScript SDK (Swell.js), headless storefront starters for Next.js (Horizon, verswell-commerce, nextjs-commerce) and Nuxt (Origin), a Swell Apps platform with CLI and Apps SDK for extending the data and logic layers via custom data models, events, notifications, webhooks, and edge functions running in 200+ locations, plus AI coding-agent skills and Claude Code plugins.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/apis.yml)

## Tags

- Commerce
- Headless Commerce
- API-First
- B2C
- B2B
- Subscriptions
- Marketplaces
- Wholesale
- Storefront
- Checkout
- Payments
- Carts
- Orders
- Catalog
- Internationalization

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Swell Backend API

Server-side REST API authorized with a secret API key and store ID. Covers products, variants, stock, categories, attributes, purchase links, carts, orders, payments, refunds, shipments, returns, subscriptions, subscription plans, accounts, addresses, cards, credits, invoices, coupons, promotions, gift cards, content pages, files, events, and webhooks. Supports MongoDB-style `where` filters with operators ($eq, $ne, $gt, $gte, $lt, $lte, $in, $nin, $regex, $type, $exists, $and, $or, $nor, $all, $elemMatch, $size), `sort`, `limit` (1-1000, default 15), `page`, `search`, `expand`, `fields`, and `include`. Official libraries connect over a custom wire protocol on port 8443 for improved performance and caching; HTTPS REST is available at api.swell.store.

- **Human URL:** [https://developers.swell.is/backend-api/introduction](https://developers.swell.is/backend-api/introduction)
- **Base URL:** `https://api.swell.store`

#### Tags

- Commerce
- Backend
- REST
- Catalog
- Orders
- Payments
- Subscriptions

#### Properties

- [Documentation](https://developers.swell.is/backend-api/introduction)
- [Authentication](https://developers.swell.is/backend-api/authentication)
- [API Reference](https://developers.swell.is/backend-api/querying)
- [API Reference](https://developers.swell.is/backend-api/errors)
- [OpenAPI](openapi/swell-backend-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/swell-backend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-backend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/swell-product-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-cart-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-subscription-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-payment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/swell-webhook-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/swell-product-structure.json)
- [JSON Structure](json-structure/swell-order-structure.json)
- [JSON Structure](json-structure/swell-subscription-structure.json)
- [JSON Structure](json-structure/swell-account-structure.json)
- [Example](examples/swell-product-create-example.json)
- [Example](examples/swell-order-create-example.json)
- [Example](examples/swell-subscription-create-example.json)
- [Example](examples/swell-account-create-example.json)
- [Example](examples/swell-webhook-event-example.json)

### Swell Frontend API

Public-key-authorized REST API designed for storefronts, JAMstack apps, and SSR frameworks. Powers Swell.js and the official Next.js (Horizon, verswell-commerce, nextjs-commerce, nextjs-builder) and Nuxt (Origin) headless starters. Exposes products, categories, attributes, carts (with coupon and gift-card application, recovery, and order submission), authenticated customer accounts (login, recovery, addresses, cards, orders, subscriptions), store settings, payment settings, currencies, menus, and content models. Authenticated with a public key (pk_...) and a session token making it safe to use from any client context.

- **Human URL:** [https://developers.swell.is/frontend-api/introduction](https://developers.swell.is/frontend-api/introduction)
- **Base URL:** `https://{store-id}.swell.store`

#### Tags

- Commerce
- Frontend
- Storefront
- REST
- JAMstack

#### Properties

- [Documentation](https://developers.swell.is/frontend-api/introduction)
- [OpenAPI](openapi/swell-frontend-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/swell-frontend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-frontend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/swell-cart-add-item-example.json)

### Swell GraphQL API

Experimental (alpha) GraphQL endpoint that exposes a curated subset of the storefront commerce model — products, attributes, categories, accounts, sessions, carts, orders, payments, payment settings, subscriptions, store settings, currencies, and navigation menus. Authorized with a public storefront key passed in the Authorization header. Notable limits: no nested queries, no payment tokenization, no abandoned-cart recovery, no guest cart email updates. A GraphQL playground is available at /playground when logged into the dashboard.

- **Human URL:** [https://developers.swell.is/frontend-api/frontend-libraries/graphql](https://developers.swell.is/frontend-api/frontend-libraries/graphql)
- **Base URL:** `https://{store-id}.swell.store/graphql/v2`

#### Tags

- Commerce
- GraphQL
- Storefront
- Experimental

#### Properties

- [Documentation](https://developers.swell.is/frontend-api/frontend-libraries/graphql)
- [API Reference](https://{store-id}.swell.store/playground)
- [Postman Collection](collections/swell-backend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-backend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/swell-frontend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-frontend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Swell Webhooks

Event-driven HTTP callbacks for cart, order, subscription, payment, account, and product lifecycle events. Configurable via the dashboard (Developer → Webhooks) or programmatically through the Backend API and Swell Apps. Payloads are JSON POSTs with `id`, `date_created`, `model`, `type`, and `data`. Endpoints must return 2xx; failed deliveries retry hourly for two days, continue hourly after, and auto-disable after three days. Webhooks originate from the documented Swell IP allowlist (52.52.111.237, 54.219.85.17, 54.241.235.166, plus 216.218.185.0/27, 216.218.244.192/27, 74.80.234.0/24).

- **Human URL:** [https://developers.swell.is/backend-api/webhooks](https://developers.swell.is/backend-api/webhooks)

#### Tags

- Commerce
- Eventing
- Webhooks

#### Properties

- [Documentation](https://developers.swell.is/backend-api/webhooks)
- [Example](examples/swell-webhook-event-example.json)
- [Postman Collection](collections/swell-backend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-backend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/swell-frontend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-frontend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Swell Apps Platform

Swell Apps extend the platform with custom data models (added fields or new entities), events (triggering functions, webhooks, and notifications), edge functions deployed to 200+ locations with no cold start, and admin UI surfaces (settings, content views). Apps are distributed via a swell.json manifest and built with the Swell CLI and Apps SDK; TypeScript bindings are published in the app-types package. Used for first-party integrations (Contentful, Builder.io, honest reviews) and third-party merchant extensions.

- **Human URL:** [https://developers.swell.is/apps/overview](https://developers.swell.is/apps/overview)

#### Tags

- Apps
- Extensions
- Functions
- Edge

#### Properties

- [Documentation](https://developers.swell.is/apps/overview)
- [SDK](https://github.com/swellstores/apps-sdk)
- [SDK](https://github.com/swellstores/app-types)
- [Postman Collection](collections/swell-backend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-backend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/swell-frontend-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/swell-frontend-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Homepage](https://www.swell.is/)
- [Developer Portal](https://www.swell.is/)
- [Documentation](https://developers.swell.is)
- [Quickstart](https://developers.swell.is/guides/quickstart-guide)
- [Getting Started](https://developers.swell.is/guides/core-concepts/platform-overview)
- [Features](https://www.swell.is/features)
- [Pricing](https://www.swell.is/pricing)
- [Sign Up](https://swell.store/signup)
- [Login](https://swell.store/admin/login)
- [Console](https://swell.store/admin)
- [Status Page](https://status.swell.store/)
- [Changelog](https://www.swell.is/changelog)
- [Blog](https://www.swell.is/blog)
- [Support](https://www.swell.is/help)
- [Contact](https://www.swell.is/contact)
- [Terms of Service](https://www.swell.is/legal/terms-of-service)
- [Privacy Policy](https://www.swell.is/legal/privacy-policy)
- [GitHub Organization](https://github.com/swellstores)
- [Forum](https://github.com/orgs/swellstores/discussions)
- [X (Twitter)](https://x.com/swellcommerce)
- [LinkedIn](https://www.linkedin.com/company/swellcommerce/)
- [SDK](https://github.com/swellstores/swell-node)
- [SDK](https://github.com/swellstores/swell-php)
- [SDK](https://github.com/swellstores/swell-js)
- [SDK](https://github.com/swellstores/swellpy)
- [SDK](https://github.com/swellstores/apps-sdk)
- [SDK](https://github.com/swellstores/app-types)
- [Resources](https://github.com/swellstores/horizon)
- [Resources](https://github.com/swellstores/origin-theme)
- [Resources](https://github.com/swellstores/verswell-commerce)
- [Resources](https://github.com/swellstores/nextjs-commerce)
- [Resources](https://github.com/swellstores/nextjs-builder)
- [Resources](https://github.com/swellstores/storefront-react-ai-template)
- [Resources](https://github.com/swellstores/swell-claude-plugins)
- [Resources](https://github.com/swellstores/skills)
- [Resources](https://github.com/swellstores/easyblocks)
- [Resources](https://github.com/swellstores/proxima-app)
- [Resources](https://github.com/swellstores/contentful-app)
- [Resources](https://github.com/swellstores/honest-reviews-app)
- [Resources](https://github.com/swellstores/community)
- [Spectral Rules](rules/swell-rules.yml)
- [Vocabulary](vocabulary/swell-io-vocabulary.yml)
- [JSON-LD](json-ld/swell-io-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/swell-io-plans-pricing.yml)
- [Rate Limits](rate-limits/swell-io-rate-limits.yml)
- [Fin Ops](finops/swell-io-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://kinlane.com
