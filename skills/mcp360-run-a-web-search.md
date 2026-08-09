---
name: Run a web search across engines
description: Query Google, Bing or DuckDuckGo through one gateway and normalize the results, including
  localized and time-boxed searches.
api: openapi/mcp360-google-search-openapi.json
operations:
- google-search_search_web
- google-search_search_advanced
- google-search_get_autocomplete
- google-search_get_related_searches
- bing-search_search_web
- bing-search_search_news
- duckduckgo-search_search_web
---

# Run a web search across engines

> Query Google, Bing or DuckDuckGo through one gateway and normalize the results, including localized and time-boxed searches.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-google-search-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
The caller needs live SERP data — general web results, news, autocomplete, or "what else do people search for".

## Steps

1. **Pick the engine.** `google-search` for general/organic depth, `bing-search` when you also need `search_news`, `search_images` or `search_local`, `duckduckgo-search` for a lighter unpersonalized read.
2. **Search.** `POST /api/v1/google-search/search_web` (`google-search_search_web`). Required: `query` (1-2048 chars). Optional and worth setting:
   - `location` — city or state name **only, no commas** ("New York", not "New York, NY"). This is the most common 400.
   - `country` — exactly two lowercase letters (`^[a-z]{2}$`), e.g. `us`, `uk`.
   - `language` — `^[a-z]{2}(-[a-z]{2})?$`, e.g. `en`, `en-gb`.
   - `num_results` — integer 1-100, default 10.
   - `safe_search` — boolean, default false.
   - `time_period` — a single char from `h|d|w|m|y` (hour/day/week/month/year).
3. **Expand the query** when results are thin: `google-search_get_autocomplete` for query completions and `google-search_get_related_searches` for adjacent intents. Feed the best back into step 2.
4. **Go deeper** with `google-search_search_advanced` when you need operator-level control.
5. **Read the results.** `data` carries `organic[]` plus `ads[]` (with `link`, `title`, `domain`, `rating`, `source`) — separate paid from organic before reporting.

## Watch out
- `num_results: 100` costs the same credits as `10`; ask for what you will actually read.
- Each engine returns its own shape. Normalize on `title` / `link` / `domain` and treat everything else as engine-specific.
