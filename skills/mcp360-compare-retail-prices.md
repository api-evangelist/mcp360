---
name: Compare product prices across retailers
description: Search Amazon, Walmart, eBay and Google Shopping through one gateway and produce a like-for-like
  price comparison.
api: openapi/mcp360-google-shopping-openapi.json
operations:
- amazon-search_search_products
- amazon-search_get_product_details
- amazon-search_find_product_position
- amazon-search_bulk_find_product_position
- walmart-search_search_products
- walmart-search_get_product_details
- ebay-search_search_products
- ebay-search_search_auctions
- ebay-search_get_product_details
- google-shopping_search_products
- google-shopping_compare_prices
- google-shopping_filter_by_price_range
- google-shopping_get_product_details
---

# Compare product prices across retailers

> Search Amazon, Walmart, eBay and Google Shopping through one gateway and produce a like-for-like price comparison.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-google-shopping-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
The caller wants a price on a product, or wants to know who sells it cheapest.

## Steps

1. **Start broad.** `google-shopping_search_products` or `google-shopping_compare_prices` gives you a cross-retailer read in one call — use it before hitting individual marketplaces.
2. **Go per-retailer** for depth: `amazon-search_search_products`, `walmart-search_search_products`, `ebay-search_search_products`. For eBay also run `ebay-search_search_auctions` — auction pricing is a different market from buy-it-now and mixing them produces a false low.
3. **Resolve the exact item.** A search hit is not a match. Call `{retailer}_get_product_details` on the candidate before quoting a price, and confirm it is the same model/variant.
4. **Narrow by budget** with `google-shopping_filter_by_price_range` when the caller gave one.
5. **Merchandising questions** ("where do we show up for this term") use `amazon-search_find_product_position`, or `amazon-search_bulk_find_product_position` for a keyword list.

## Watch out
- Prices exclude shipping and tax unless the retailer's payload says otherwise. Say so when you report.
- `amazon-search_search_prime_products` filters to Prime-eligible only — that is a different population, not a sort order.
- Never quote a price from a search listing alone; confirm with `get_product_details`.
