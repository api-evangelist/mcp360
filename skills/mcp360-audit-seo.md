---
name: Audit a site's SEO position
description: Combine keyword volume, on-page checks and rank tracking to produce a grounded SEO read for
  a domain.
api: openapi/mcp360-onpage-seo-openapi.json
operations:
- keyword-research_search_keyword_volume
- keyword-research_global_keyword_volume
- keyword-research_related_keyword_suggestions
- onpage-seo_single_onpage_checker
- onpage-seo_bulk_onpage_checker
- google-rank-tracking_get_search_results
- google-rank-tracking_find_domain_position
- google-rank-tracking_bulk_find_domain_position
---

# Audit a site's SEO position

> Combine keyword volume, on-page checks and rank tracking to produce a grounded SEO read for a domain.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-onpage-seo-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
The caller wants to know how a site is performing in search and what to fix.

## Steps

1. **Build the keyword set.** `keyword-research_search_keyword_volume` for the seeds you were given, then `keyword-research_related_keyword_suggestions` to widen. Use `keyword-research_global_keyword_volume` when the question is not country-specific.
2. **Check the pages.** `onpage-seo_single_onpage_checker` for one URL; `onpage-seo_bulk_onpage_checker` when auditing a set — do not loop the single-URL tool.
3. **Find where the domain actually ranks.** `google-rank-tracking_find_domain_position` per keyword, or `google-rank-tracking_bulk_find_domain_position` for the whole keyword set in one call. `google-rank-tracking_get_search_results` gives you the full SERP when you need to see who is above them.
4. **Report** ranking positions against volume — a rank-3 for a 50/mo keyword is not the same win as a rank-9 for a 40,000/mo keyword. Never present position without volume.

## Watch out
- Rank data is a point-in-time sample from one location. State the `location`/`country` you queried with alongside every position you report.
- The bulk tools are the difference between one credit-efficient audit and a hundred separate charges.
