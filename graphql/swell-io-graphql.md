# Swell GraphQL API

Experimental (alpha) GraphQL endpoint that exposes a curated subset of the storefront commerce model — products, attributes, categories, accounts, sessions, carts, orders, payments, payment settings, subscriptions, store settings, currencies, and navigation menus. Authorized with a public storefront key passed in the Authorization header. Notable limits: no nested queries, no payment tokenization, no abandoned-cart recovery, no guest cart email updates. A GraphQL playground is available at /playground when logged into the dashboard.

**Endpoint:** https://{store-id}.swell.store/graphql/v2

**Documentation:** https://developers.swell.is/frontend-api/frontend-libraries/graphql

**References:**

- Documentation: https://developers.swell.is/frontend-api/frontend-libraries/graphql
- APIReference: https://{store-id}.swell.store/playground
