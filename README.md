# MCP360

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

MCP360 is a hosted unified Model Context Protocol gateway operated by Delta4 Infotech Pvt. Ltd. that gives AI agents access to 38 tool services — 106 individual tools — through a single credentialed endpoint, plus a no-code Custom MCP Builder that wraps any REST API as an MCP server. Every service is exposed twice: as a hosted remote MCP server at connect.mcp360.ai/v1/{service}/mcp and as a conventional REST API at connect.mcp360.ai/api/v1/{service}/{tool}, both generated from one tool registry. The gateway serves a machine-generated OpenAPI 3.0.0 document per service at /api/v1/{service}/openapi.json and publishes every tool input and output JSON Schema anonymously at /api/v1/{service}. Coverage spans search engines (Google, Bing, DuckDuckGo, Baidu, Yandex, Yahoo, Naver), Google verticals (Maps, News, Trends, Scholar, Flights, Hotels, Jobs, Shopping, Images, Play), retail (Amazon, Walmart, eBay), SEO (keyword research, on-page audit, rank tracking), and infrastructure lookups (WHOIS, DNS, IP, URL, email verification, web scraping). Auth is an API key via X-API-Key or bearer token, with OAuth 2.1 (authorization code, PKCE S256, dynamic client registration) for the MCP surface. Billing is monthly credits.

**Areas:** MCP · MCP Server · MCP Gateway · AI Agents · Agent Tools · Tool Integration · Unified API · API Gateway · No-Code · llms-txt · SEO · Search

## MCP360 on APIs.io

Everything profiled for MCP360 is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/mcp360/](https://apis.io/providers/mcp360/)** — or go straight to one of the APIs or properties below.

### APIs (38)

- [MCP360 Amazon Search API](https://apis.io/apis/mcp360/mcp360-amazon-search-api/) — The amazon-search API from MCP360 — 6 operation(s) for amazon-search.
- [MCP360 Apple Appstore API](https://apis.io/apis/mcp360/mcp360-apple-appstore-api/) — The apple-appstore API from MCP360 — 4 operation(s) for apple-appstore.
- [MCP360 Baidu Search API](https://apis.io/apis/mcp360/mcp360-baidu-search-api/) — The baidu-search API from MCP360 — 3 operation(s) for baidu-search.
- [MCP360 Bing Search API](https://apis.io/apis/mcp360/mcp360-bing-search-api/) — The bing-search API from MCP360 — 4 operation(s) for bing-search.
- [MCP360 Cryptocurrency API](https://apis.io/apis/mcp360/mcp360-cryptocurrency-api/) — The cryptocurrency API from MCP360 — 2 operation(s) for cryptocurrency.
- [MCP360 Currency Converter API](https://apis.io/apis/mcp360/mcp360-currency-converter-api/) — The currency-converter API from MCP360 — 1 operation(s) for currency-converter.
- [MCP360 Dns Lookup API](https://apis.io/apis/mcp360/mcp360-dns-lookup-api/) — The dns-lookup API from MCP360 — 2 operation(s) for dns-lookup.
- [MCP360 Duckduckgo Search API](https://apis.io/apis/mcp360/mcp360-duckduckgo-search-api/) — The duckduckgo-search API from MCP360 — 1 operation(s) for duckduckgo-search.
- [MCP360 Ebay Search API](https://apis.io/apis/mcp360/mcp360-ebay-search-api/) — The ebay-search API from MCP360 — 3 operation(s) for ebay-search.
- [MCP360 Email Verification API](https://apis.io/apis/mcp360/mcp360-email-verification-api/) — The email-verification API from MCP360 — 2 operation(s) for email-verification.
- [MCP360 Google Flights API](https://apis.io/apis/mcp360/mcp360-google-flights-api/) — The google-flights API from MCP360 — 3 operation(s) for google-flights.
- [MCP360 Google Forums API](https://apis.io/apis/mcp360/mcp360-google-forums-api/) — The google-forums API from MCP360 — 1 operation(s) for google-forums.
- [MCP360 Google Hotels API](https://apis.io/apis/mcp360/mcp360-google-hotels-api/) — The google-hotels API from MCP360 — 1 operation(s) for google-hotels.
- [MCP360 Google Images API](https://apis.io/apis/mcp360/mcp360-google-images-api/) — The google-images API from MCP360 — 1 operation(s) for google-images.
- [MCP360 Google Jobs API](https://apis.io/apis/mcp360/mcp360-google-jobs-api/) — The google-jobs API from MCP360 — 1 operation(s) for google-jobs.
- [MCP360 Google Maps API](https://apis.io/apis/mcp360/mcp360-google-maps-api/) — The google-maps API from MCP360 — 4 operation(s) for google-maps.
- [MCP360 Google News API](https://apis.io/apis/mcp360/mcp360-google-news-api/) — The google-news API from MCP360 — 2 operation(s) for google-news.
- [MCP360 Google Play API](https://apis.io/apis/mcp360/mcp360-google-play-api/) — The google-play API from MCP360 — 2 operation(s) for google-play.
- [MCP360 Google Rank Tracking API](https://apis.io/apis/mcp360/mcp360-google-rank-tracking-api/) — The google-rank-tracking API from MCP360 — 3 operation(s) for google-rank-tracking.
- [MCP360 Google Scholar API](https://apis.io/apis/mcp360/mcp360-google-scholar-api/) — The google-scholar API from MCP360 — 4 operation(s) for google-scholar.
- [MCP360 Google Search API](https://apis.io/apis/mcp360/mcp360-google-search-api/) — The google-search API from MCP360 — 4 operation(s) for google-search.
- [MCP360 Google Shopping API](https://apis.io/apis/mcp360/mcp360-google-shopping-api/) — The google-shopping API from MCP360 — 4 operation(s) for google-shopping.
- [MCP360 Google Trends API](https://apis.io/apis/mcp360/mcp360-google-trends-api/) — The google-trends API from MCP360 — 3 operation(s) for google-trends.
- [MCP360 Imginny API](https://apis.io/apis/mcp360/mcp360-imginny-api/) — The imginny API from MCP360 — 4 operation(s) for imginny.
- [MCP360 Ip Info API](https://apis.io/apis/mcp360/mcp360-ip-info-api/) — The ip-info API from MCP360 — 2 operation(s) for ip-info.
- [MCP360 Keyword Research API](https://apis.io/apis/mcp360/mcp360-keyword-research-api/) — The keyword-research API from MCP360 — 3 operation(s) for keyword-research.
- [MCP360 Llm Prompt Tracker API](https://apis.io/apis/mcp360/mcp360-llm-prompt-tracker-api/) — The llm-prompt-tracker API from MCP360 — 2 operation(s) for llm-prompt-tracker.
- [MCP360 API](https://apis.io/apis/mcp360/mcp360-mcp360-api/) — The mcp360 API from MCP360 — 2 operation(s) for mcp360.
- [MCP360 Naver Search API](https://apis.io/apis/mcp360/mcp360-naver-search-api/) — The naver-search API from MCP360 — 3 operation(s) for naver-search.
- [MCP360 Onpage Seo API](https://apis.io/apis/mcp360/mcp360-onpage-seo-api/) — The onpage-seo API from MCP360 — 2 operation(s) for onpage-seo.
- [MCP360 URL Lookup API](https://apis.io/apis/mcp360/mcp360-url-lookup-api/) — The url-lookup API from MCP360 — 2 operation(s) for url-lookup.
- [MCP360 Walmart Search API](https://apis.io/apis/mcp360/mcp360-walmart-search-api/) — The walmart-search API from MCP360 — 2 operation(s) for walmart-search.
- [MCP360 Weather API](https://apis.io/apis/mcp360/mcp360-weather-api/) — The weather API from MCP360 — 3 operation(s) for weather.
- [MCP360 Web Scraping API](https://apis.io/apis/mcp360/mcp360-web-scraping-api/) — The web-scraping API from MCP360 — 1 operation(s) for web-scraping.
- [MCP360 Whois API](https://apis.io/apis/mcp360/mcp360-whois-api/) — The whois API from MCP360 — 3 operation(s) for whois.
- [MCP360 Yahoo Search API](https://apis.io/apis/mcp360/mcp360-yahoo-search-api/) — The yahoo-search API from MCP360 — 3 operation(s) for yahoo-search.
- [MCP360 Yandex Search API](https://apis.io/apis/mcp360/mcp360-yandex-search-api/) — The yandex-search API from MCP360 — 3 operation(s) for yandex-search.
- [MCP360 Youtube API](https://apis.io/apis/mcp360/mcp360-youtube-api/) — The youtube API from MCP360 — 10 operation(s) for youtube.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [MCP360 Unified Gateway](https://apis.io/servers/mcp360/mcp360-unified-gateway/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Mcp360 Agentic Access](https://apis.io/agentic-access/mcp360/mcp360-agentic-access/)

#### JSON Schema (1)

The data models the API reads and writes.

- [MCP360 tool input/output schemas](https://apis.io/schemas/mcp360/mcp360-tool-schemas/)

#### Collections (38)

Postman and Open Collection request collections.

- [Amazon Product Search Tools REST Amazon Search API](https://apis.io/collections/mcp360/open-mcp360-amazon-search-api/)
- [Apple App Store Tools REST Apple Appstore API](https://apis.io/collections/mcp360/open-mcp360-apple-appstore-api/)
- [Tools REST Baidu Search API](https://apis.io/collections/mcp360/open-mcp360-baidu-search-api/)
- [Tools REST Bing Search API](https://apis.io/collections/mcp360/open-mcp360-bing-search-api/)
- [Service REST Cryptocurrency API](https://apis.io/collections/mcp360/open-mcp360-cryptocurrency-api/)
- [Service REST Currency Converter API](https://apis.io/collections/mcp360/open-mcp360-currency-converter-api/)
- [Service REST Dns Lookup API](https://apis.io/collections/mcp360/open-mcp360-dns-lookup-api/)
- [Tools REST Duckduckgo Search API](https://apis.io/collections/mcp360/open-mcp360-duckduckgo-search-api/)
- [eBay Product Search Tools REST Ebay Search API](https://apis.io/collections/mcp360/open-mcp360-ebay-search-api/)
- [Tools REST Email Verification API](https://apis.io/collections/mcp360/open-mcp360-email-verification-api/)
- [Tools REST Google Flights API](https://apis.io/collections/mcp360/open-mcp360-google-flights-api/)
- [Tools REST Google Forums API](https://apis.io/collections/mcp360/open-mcp360-google-forums-api/)
- [Tools REST Google Hotels API](https://apis.io/collections/mcp360/open-mcp360-google-hotels-api/)
- [Tools REST Google Images API](https://apis.io/collections/mcp360/open-mcp360-google-images-api/)
- [Tools REST Google Jobs API](https://apis.io/collections/mcp360/open-mcp360-google-jobs-api/)
- [Tools REST Google Maps API](https://apis.io/collections/mcp360/open-mcp360-google-maps-api/)
- [Tools REST Google News API](https://apis.io/collections/mcp360/open-mcp360-google-news-api/)
- [Store Tools REST Google Play API](https://apis.io/collections/mcp360/open-mcp360-google-play-api/)
- [Tools REST Google Rank Tracking API](https://apis.io/collections/mcp360/open-mcp360-google-rank-tracking-api/)
- [Tools REST Google Scholar API](https://apis.io/collections/mcp360/open-mcp360-google-scholar-api/)
- [Tools REST Google Search API](https://apis.io/collections/mcp360/open-mcp360-google-search-api/)
- [Tools REST Google Shopping API](https://apis.io/collections/mcp360/open-mcp360-google-shopping-api/)
- [Tools REST Google Trends API](https://apis.io/collections/mcp360/open-mcp360-google-trends-api/)
- [AI Image Generation REST Imginny API](https://apis.io/collections/mcp360/open-mcp360-imginny-api/)
- [IP Information Tools REST Ip Info API](https://apis.io/collections/mcp360/open-mcp360-ip-info-api/)
- …and 13 more published on APIs.io

#### Overlays (38)

OpenAPI overlays, including conversational phrasing for each operation.

- [Mcp360 Amazon Search Overlay](https://apis.io/overlays/mcp360/mcp360-amazon-search-overlay/)
- [Mcp360 Apple Appstore Overlay](https://apis.io/overlays/mcp360/mcp360-apple-appstore-overlay/)
- [Mcp360 Baidu Search Overlay](https://apis.io/overlays/mcp360/mcp360-baidu-search-overlay/)
- [Mcp360 Bing Search Overlay](https://apis.io/overlays/mcp360/mcp360-bing-search-overlay/)
- [Mcp360 Cryptocurrency Overlay](https://apis.io/overlays/mcp360/mcp360-cryptocurrency-overlay/)
- [Mcp360 Currency Converter Overlay](https://apis.io/overlays/mcp360/mcp360-currency-converter-overlay/)
- [Mcp360 Dns Lookup Overlay](https://apis.io/overlays/mcp360/mcp360-dns-lookup-overlay/)
- [Mcp360 Duckduckgo Search Overlay](https://apis.io/overlays/mcp360/mcp360-duckduckgo-search-overlay/)
- [Mcp360 Ebay Search Overlay](https://apis.io/overlays/mcp360/mcp360-ebay-search-overlay/)
- [Mcp360 Email Verification Overlay](https://apis.io/overlays/mcp360/mcp360-email-verification-overlay/)
- [Mcp360 Google Flights Overlay](https://apis.io/overlays/mcp360/mcp360-google-flights-overlay/)
- [Mcp360 Google Forums Overlay](https://apis.io/overlays/mcp360/mcp360-google-forums-overlay/)
- [Mcp360 Google Hotels Overlay](https://apis.io/overlays/mcp360/mcp360-google-hotels-overlay/)
- [Mcp360 Google Images Overlay](https://apis.io/overlays/mcp360/mcp360-google-images-overlay/)
- [Mcp360 Google Jobs Overlay](https://apis.io/overlays/mcp360/mcp360-google-jobs-overlay/)
- [Mcp360 Google Maps Overlay](https://apis.io/overlays/mcp360/mcp360-google-maps-overlay/)
- [Mcp360 Google News Overlay](https://apis.io/overlays/mcp360/mcp360-google-news-overlay/)
- [Mcp360 Google Play Overlay](https://apis.io/overlays/mcp360/mcp360-google-play-overlay/)
- [Mcp360 Google Rank Tracking Overlay](https://apis.io/overlays/mcp360/mcp360-google-rank-tracking-overlay/)
- [Mcp360 Google Scholar Overlay](https://apis.io/overlays/mcp360/mcp360-google-scholar-overlay/)
- [Mcp360 Google Search Overlay](https://apis.io/overlays/mcp360/mcp360-google-search-overlay/)
- [Mcp360 Google Shopping Overlay](https://apis.io/overlays/mcp360/mcp360-google-shopping-overlay/)
- [Mcp360 Google Trends Overlay](https://apis.io/overlays/mcp360/mcp360-google-trends-overlay/)
- [Mcp360 Imginny Overlay](https://apis.io/overlays/mcp360/mcp360-imginny-overlay/)
- [Mcp360 Ip Info Overlay](https://apis.io/overlays/mcp360/mcp360-ip-info-overlay/)
- …and 13 more published on APIs.io

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Mcp360 Authentication](https://apis.io/security/mcp360/mcp360-authentication/)
- [Mcp360 Domain Security](https://apis.io/security/mcp360/mcp360-domain-security/)
- [Mcp360 Vulnerability Disclosure](https://apis.io/security/mcp360/mcp360-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Mcp360 Scopes](https://apis.io/scopes/mcp360/mcp360-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Mcp360 Plans](https://apis.io/plans/mcp360/mcp360-plans/)

#### Rate limits (1)

Published request limits.

- [Mcp360 Rate Limits](https://apis.io/rate-limits/mcp360/mcp360-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.mcp360.ai/)
- [Documentation](https://mcp360.ai/docs)
- [Getting started](https://mcp360.ai/docs)
- [Pricing](https://mcp360.ai/pricing)
- [Sign up](https://dashboard.mcp360.ai/signup)
- [Support](https://mcp360.ai/contact)
- [Blog](https://mcp360.ai/blog)
- [Security](https://github.com/mcp360/mTarsier/blob/HEAD/SECURITY.md)
- [Terms of service](https://mcp360.ai/terms)
- [Privacy policy](https://mcp360.ai/privacy)
- [GitHub](https://github.com/mcp360)

## API Evangelist rating

**Kin Score 51.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 47.9 |
| Contract governance | 4.5 |
| Operational transparency | 13.2 |
| Developer ergonomics | 63.7 |
| Access clarity | 69.7 |

**Agent readiness 21.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | — |

**Regulatory alignment 40.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/mcp360/](https://apis.io/providers/mcp360/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for MCP360: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/mcp360/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
