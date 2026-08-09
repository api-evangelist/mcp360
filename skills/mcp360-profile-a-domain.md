---
name: Profile a domain end to end
description: Chain WHOIS, DNS, IP and URL tools to build a full picture of a domain — ownership, hosting,
  mail path and liveness.
api: openapi/mcp360-whois-openapi.json
operations:
- whois_lookup_domain
- whois_check_availability
- whois_bulk_check_availability
- dns-lookup_lookup_dns
- dns-lookup_lookup_mx
- ip-info_get_ip_info
- ip-info_batch_ip_lookup
- url-lookup_validate_url
- url-lookup_get_webpage_info
---

# Profile a domain end to end

> Chain WHOIS, DNS, IP and URL tools to build a full picture of a domain — ownership, hosting, mail path and liveness.

Gateway: `https://connect.mcp360.ai` — every operation below is a real `operationId` in `openapi/mcp360-whois-openapi.json` (or the sibling service spec in `openapi/`).

## Conventions that apply to every call

- **Auth:** send `X-API-Key: <key>` (or `Authorization: Bearer <key>`). Keys come from https://dashboard.mcp360.ai -> Settings -> API Keys. A missing *and* an invalid key both return **401** with `{"error":"Authentication failed", ...}` — read `message` to tell them apart.
- **Shape:** every tool is `POST https://connect.mcp360.ai/api/v1/{service}/{tool}` with a JSON body. Most tools also expose a `GET` twin (`operationId` suffix `_get`) for query-string calls.
- **Validate before you send.** Every input schema is `additionalProperties: false` — an unknown key is a **400**. The authoritative schemas are in `json-schema/mcp360-tool-schemas.json`.
- **Response:** `{"success": bool, "data": {...}, "metadata": {...}}`. Add `?includeMetadata=true` to get `creditsUsed`, `executionTime` and `timestamp` back. Add `?validateOutput=true` (and `?strictValidation=true` to hard-fail) to check the payload against the tool's published `outputSchema`.
- **Billing:** every call costs credits (1 per use on all services captured). Failed calls are not charged. Quota is monthly credits per plan — see `plans/mcp360-plans.yml`.
- **No idempotency key, no request-id header, and no rate-limit headers.** Do not assume safe replay on write-shaped tools; do not expect `Retry-After` on throttling.
- **Errors:** bespoke `{"error","message","hint"}` JSON, not RFC 9457. See `errors/mcp360-problem-types.yml`.

## When to use this
Due diligence on a domain: who owns it, where it is hosted, whether it accepts mail, whether the site is live.

## Steps

1. **Ownership and dates.** `POST /api/v1/whois/lookup_domain` (`whois_lookup_domain`) — registrar, registration and expiry dates, nameservers.
2. **Availability** (for a domain that may not be registered): `whois_check_availability`, or `whois_bulk_check_availability` when you are screening a list. Always prefer the bulk tool over a loop — one call, one credit charge pattern, no partial-failure bookkeeping.
3. **DNS.** `dns-lookup_lookup_dns` for the record set, `dns-lookup_lookup_mx` for the mail path. An empty MX is a strong signal the domain does not receive mail.
4. **Hosting.** Take the resolved A record and call `ip-info_get_ip_info` for geo/ASN/org, or `ip-info_batch_ip_lookup` for several at once.
5. **Liveness and content.** `url-lookup_validate_url` to confirm the URL resolves, then `url-lookup_get_webpage_info` for title/metadata.

## Watch out
- Use the `bulk_*` / `batch_*` variants whenever you have more than a couple of inputs — they exist on `whois`, `ip-info` and `email-verification`.
- WHOIS privacy services mean an absent registrant is normal, not an error. Do not report "no owner" as a finding.
