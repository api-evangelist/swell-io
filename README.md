# Swell (swell-io)

Swell is a customizable, API-first headless commerce platform powering modern B2C, B2B, subscription, and marketplace experiences. It exposes a server-side Backend API for the full commerce data model, a public-key Frontend API for storefronts, an experimental GraphQL endpoint, and a Swell Apps platform for extending data, logic, and admin UI via edge functions. Official Node and PHP libraries, the universal Swell.js SDK, and headless storefront starters for Next.js (Horizon, verswell-commerce) and Nuxt (Origin) round out the developer surface.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Commerce, Headless Commerce, API-First, B2C, B2B, Subscriptions, Marketplaces, Wholesale, Storefront, Checkout, Payments, Carts, Orders, Catalog, Internationalization

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## At a Glance

| Item | Value |
|---|---|
| Architecture | Headless, API-first commerce |
| Models | B2C, B2B / wholesale, subscriptions, marketplaces, omnichannel |
| Backend API base URL | `https://api.swell.store` |
| Frontend API base URL | `https://{store-id}.swell.store` |
| GraphQL endpoint | `https://{store-id}.swell.store/graphql/v2` (alpha) |
| Auth | Secret key (`sk_...`) for Backend; public key (`pk_...`) for Frontend |
| Wire protocol | Custom protocol on port 8443 (via official Node and PHP libraries) |
| Pagination | `limit` 1-1000 (default 15), `page`, MongoDB-style `where` filters |
| Internationalization | 230 currencies, 170 languages |
| Pricing | Starter $29/mo → Unlimited $2,250/mo + Custom enterprise |
| Status page | https://status.swell.store |

## APIs

### Swell Backend API
Server-side REST API for the full commerce data model — products, variants, stock, categories, attributes, purchase links, carts, orders, payments, refunds, shipments, returns, subscriptions, plans, accounts, addresses, cards, credits, invoices, coupons, promotions, gift cards, content pages, files, events, and webhooks. Supports MongoDB-style `where` filters, `sort`, `limit`, `page`, `search`, `expand`, `include`, `fields`. Authorized with a store ID and secret key.

**Human URL:** [https://developers.swell.is/backend-api/introduction](https://developers.swell.is/backend-api/introduction)

- [OpenAPI](openapi/swell-backend-api-openapi.yml)
- [JSON Schema — Product](json-schema/swell-product-schema.json)
- [JSON Schema — Order](json-schema/swell-order-schema.json)
- [JSON Schema — Cart](json-schema/swell-cart-schema.json)
- [JSON Schema — Subscription](json-schema/swell-subscription-schema.json)
- [JSON Schema — Account](json-schema/swell-account-schema.json)
- [JSON Schema — Payment](json-schema/swell-payment-schema.json)
- [JSON Schema — Webhook](json-schema/swell-webhook-schema.json)
- [Example — Create Product](examples/swell-product-create-example.json)
- [Example — Create Order](examples/swell-order-create-example.json)
- [Example — Create Subscription](examples/swell-subscription-create-example.json)
- [Example — Create Account](examples/swell-account-create-example.json)
- [Example — Webhook Event](examples/swell-webhook-event-example.json)
- [Naftiko Capability — Catalog Management](capabilities/catalog-management.yaml)
- [Naftiko Capability — Order Fulfillment](capabilities/order-fulfillment.yaml)
- [Naftiko Capability — Subscription Lifecycle](capabilities/subscription-lifecycle.yaml)
- [Naftiko Capability — Customer Management](capabilities/customer-management.yaml)
- [Naftiko Capability — Discount Promotions](capabilities/discount-promotions.yaml)
- [Naftiko Capability — Webhooks](capabilities/webhooks.yaml)

### Swell Frontend API
Public-key REST API for storefronts, JAMstack apps, and SSR frameworks. Powers Swell.js and the official Next.js (Horizon, verswell-commerce, nextjs-commerce) and Nuxt (Origin) headless starters. Resources: products, categories, attributes, carts (with coupon/gift-card application, recovery, order submission), accounts (login, recovery, addresses, cards, orders, subscriptions), store settings, payment settings, currencies, menus, and content.

**Human URL:** [https://developers.swell.is/frontend-api/introduction](https://developers.swell.is/frontend-api/introduction)

- [OpenAPI](openapi/swell-frontend-api-openapi.yml)
- [Example — Add Cart Item](examples/swell-cart-add-item-example.json)
- [Naftiko Capability — Cart and Checkout](capabilities/cart-checkout.yaml)
- [Naftiko Capability — Storefront Content](capabilities/storefront-content.yaml)

### Swell GraphQL API
Experimental (alpha) GraphQL endpoint exposing a curated subset of the storefront commerce model — products, attributes, categories, accounts, sessions, carts, orders, payments, subscriptions, store settings, currencies, navigation menus. Public-key authorized. Limits: no nested queries, no payment tokenization, no abandoned-cart recovery, no guest cart email updates. GraphQL playground at `/playground`.

**Human URL:** [https://developers.swell.is/frontend-api/frontend-libraries/graphql](https://developers.swell.is/frontend-api/frontend-libraries/graphql)

### Swell Webhooks
Event-driven HTTP callbacks for cart, order, subscription, payment, account, and product lifecycle events. JSON POST with `id`, `date_created`, `model`, `type`, `data`. Endpoints must return 2xx. Retries hourly for two days, continue hourly, auto-disable after three days. Source-IP allowlist published.

**Human URL:** [https://developers.swell.is/backend-api/webhooks](https://developers.swell.is/backend-api/webhooks)

- [Example — Webhook Event](examples/swell-webhook-event-example.json)

### Swell Apps Platform
Extend Swell with custom data models, events, edge functions (200+ locations, no cold start), notifications, webhooks, and admin UI surfaces. Distributed via a `swell.json` manifest and built with the Swell CLI and Apps SDK (TypeScript bindings in `app-types`).

**Human URL:** [https://developers.swell.is/apps/overview](https://developers.swell.is/apps/overview)

## SDKs

- [Swell Node.js SDK](https://github.com/swellstores/swell-node)
- [Swell PHP SDK](https://github.com/swellstores/swell-php)
- [Swell.js Universal Storefront SDK](https://github.com/swellstores/swell-js)
- [Swellpy — community Python SDK](https://github.com/swellstores/swellpy)
- [Swell Apps SDK](https://github.com/swellstores/apps-sdk)
- [Swell Apps TypeScript Bindings](https://github.com/swellstores/app-types)

## Headless Storefront Starters

- [Horizon — Next.js](https://github.com/swellstores/horizon)
- [verswell-commerce — Next.js Commerce fork](https://github.com/swellstores/verswell-commerce)
- [Swell Next.js Commerce](https://github.com/swellstores/nextjs-commerce)
- [Swell Next.js Builder.io Starter](https://github.com/swellstores/nextjs-builder)
- [Origin Theme — Nuxt 2](https://github.com/swellstores/origin-theme)
- [Storefront React AI Template](https://github.com/swellstores/storefront-react-ai-template)

## AI Coding-Agent Resources

- [Official Claude Code Plugins for Swell](https://github.com/swellstores/swell-claude-plugins)
- [Swell AI Coding-Agent Skills](https://github.com/swellstores/skills)

## Pricing Overview

| Plan | Monthly (annual) | Annual GMV ceiling | Overage | API requests / month | Storage |
|---|---|---|---|---|---|
| Starter | $29 | $50K | 2.0% | 100K | 1 GB |
| Basic | $79 | $250K | 1.5% | 500K | 3 GB |
| Standard | $299 | $1M | 1.0% | 2M | 10 GB |
| Unlimited | $2,250 | $5M | 0.4% | Unlimited | Unlimited |
| Custom | Contact sales | $10M+ | Negotiated | Negotiated | Negotiated |

API overage: $5 per 100,000 requests. Storage overage: $5 per GB-month.

## Common Properties

- [Homepage](https://www.swell.is/)
- [Documentation](https://developers.swell.is)
- [Quickstart](https://developers.swell.is/guides/quickstart-guide)
- [Pricing](https://www.swell.is/pricing)
- [Sign Up](https://swell.store/signup)
- [Console](https://swell.store/admin)
- [Status Page](https://status.swell.store/)
- [Changelog](https://www.swell.is/changelog)
- [Blog](https://www.swell.is/blog)
- [Help Center](https://www.swell.is/help)
- [Terms of Service](https://www.swell.is/legal/terms-of-service)
- [Privacy Policy](https://www.swell.is/legal/privacy-policy)
- [GitHub Organization](https://github.com/swellstores)
- [Community Discussions](https://github.com/orgs/swellstores/discussions)
- [X / Twitter](https://x.com/swellcommerce)
- [LinkedIn](https://www.linkedin.com/company/swellcommerce/)

## Cross-Cutting Artifacts

- [Spectral Rules](rules/swell-rules.yml)
- [Vocabulary](vocabulary/swell-io-vocabulary.yml)
- [JSON-LD Context](json-ld/swell-io-context.jsonld)
- [Plans and Pricing](plans/swell-io-plans-pricing.yml)
- [Rate Limits](rate-limits/swell-io-rate-limits.yml)
- [FinOps Mapping](finops/swell-io-finops.yml)

## Maintainer

- Kin Lane — [kin@apievangelist.com](mailto:kin@apievangelist.com) — [kinlane.com](https://kinlane.com)
