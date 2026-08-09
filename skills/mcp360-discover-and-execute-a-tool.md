---
name: Discover and execute any gateway tool
description: Use the two meta-tools to find the right tool across all 38 connected services and run it,
  instead of hard-coding one service endpoint.
api: openapi/mcp360-mcp360-openapi.json
operations:
- mcp360_search
- mcp360_execute
---

# Discover and execute any gateway tool

> Use the two meta-tools to find the right tool across all 38 connected services and run it, instead of hard-coding one service endpoint.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-mcp360-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
The caller wants something done ("check if this domain is free", "what does Amazon charge for X") but you do not know which of MCP360's 38 services owns that capability. Search first, then execute — never guess a service slug.

## Steps

1. **Find the tool.** `POST /api/v1/mcp360/search` (`mcp360_search`) with `{"query": "<capability in plain words>", "limit": 10}`. `query` is 1-200 chars. The response returns `results[]` with `name`, `service`, `path`, `description`, `relevanceScore`, `matchedKeywords`, plus `matchedTools[]` and `allTools[]` — each carrying its own `schema`. Read `searchTips` and `suggestion` if `total` is 0 and re-query with different words.
2. **Read the chosen tool's schema** off `matchedTools[].schema` before building any arguments. Do not invent parameters.
3. **Run it.** `POST /api/v1/mcp360/execute` (`mcp360_execute`) with the tool identifier and the arguments you built from that schema.
4. **Or call the service directly.** Once you know the service and tool, `POST /api/v1/{service}/{tool}` is the same operation with one less hop and a spec you can validate against — prefer it for repeated calls in a loop.

## Watch out
- Enumerating services is free: `GET /api/v1/{service}` returns the full tool list with input and output schemas and needs **no credentials**. Use it to build a local index rather than burning credits on `search`.
- A bad service slug returns **404** whose body lists every valid slug in `availableServices` — use that instead of hard-coding.
