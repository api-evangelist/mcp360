---
name: Scrape and read a web page
description: Fetch page content through the gateway when the answer is on a specific URL rather than in
  a search index.
api: openapi/mcp360-web-scraping-openapi.json
operations:
- web-scraping_scrape_page
- url-lookup_get_webpage_info
- url-lookup_validate_url
---

# Scrape and read a web page

> Fetch page content through the gateway when the answer is on a specific URL rather than in a search index.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-web-scraping-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
You already have the URL and need what is on it — not a search result summary.

## Steps

1. **Validate first.** `url-lookup_validate_url` confirms the URL is well-formed and reachable. Skipping this turns a bad URL into an opaque 500 later.
2. **Cheap metadata read.** `url-lookup_get_webpage_info` when title/description/meta is enough. It costs the same credit but returns far less to parse.
3. **Full content.** `POST /api/v1/web-scraping/scrape_page` (`web-scraping_scrape_page`) for the page body.
4. **Validate the payload** with `?validateOutput=true` when you are going to parse the result programmatically.

## Watch out
- This is a live fetch against someone else's site. Respect their robots and terms; do not use it to bulk-harvest a site.
- A page that renders client-side may return a shell. If the content you expect is missing, that is the site's rendering, not a gateway error — fall back to a search tool.
