# MCP360 (mcp360)

MCP360 is a hosted unified Model Context Protocol gateway operated by Delta4 Infotech Pvt. Ltd. that gives AI agents access to 38 tool services — 106 individual tools — through a single credentialed endpoint, plus a no-code Custom MCP Builder that wraps any REST API as an MCP server. Every service is exposed twice: as a hosted remote MCP server at connect.mcp360.ai/v1/{service}/mcp and as a conventional REST API at connect.mcp360.ai/api/v1/{service}/{tool}, both generated from one tool registry. The gateway serves a machine-generated OpenAPI 3.0.0 document per service at /api/v1/{service}/openapi.json and publishes every tool input and output JSON Schema anonymously at /api/v1/{service}. Coverage spans search engines (Google, Bing, DuckDuckGo, Baidu, Yandex, Yahoo, Naver), Google verticals (Maps, News, Trends, Scholar, Flights, Hotels, Jobs, Shopping, Images, Play), retail (Amazon, Walmart, eBay), SEO (keyword research, on-page audit, rank tracking), and infrastructure lookups (WHOIS, DNS, IP, URL, email verification, web scraping). Auth is an API key via X-API-Key or bearer token, with OAuth 2.1 (authorization code, PKCE S256, dynamic client registration) for the MCP surface. Billing is monthly credits.

**APIs.json:** [https://mcp360.apievangelist.com/apis.yml](https://mcp360.apievangelist.com/apis.yml)

## Tags

- mcp
- mcp-server
- mcp-gateway
- ai-agents
- agent-tools
- tool-integration
- unified-api
- api-gateway
- no-code
- llmstxt
- seo
- search
- serp
- web-scraping
- e-commerce
- whois
- dns
- geolocation
- email-verification

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-08-09

## APIs

### MCP360 Amazon Search API

The amazon-search API from MCP360 — 6 operation(s) for amazon-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- amazon-search

#### Properties

- [OpenAPI](openapi/mcp360-amazon-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-amazon-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-amazon-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Apple Appstore API

The apple-appstore API from MCP360 — 4 operation(s) for apple-appstore.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- apple-appstore

#### Properties

- [OpenAPI](openapi/mcp360-apple-appstore-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-apple-appstore-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-apple-appstore-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Baidu Search API

The baidu-search API from MCP360 — 3 operation(s) for baidu-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- baidu-search

#### Properties

- [OpenAPI](openapi/mcp360-baidu-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-baidu-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-baidu-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Bing Search API

The bing-search API from MCP360 — 4 operation(s) for bing-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- bing-search

#### Properties

- [OpenAPI](openapi/mcp360-bing-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-bing-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-bing-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Cryptocurrency API

The cryptocurrency API from MCP360 — 2 operation(s) for cryptocurrency.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- cryptocurrency

#### Properties

- [OpenAPI](openapi/mcp360-cryptocurrency-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-cryptocurrency-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-cryptocurrency-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Currency Converter API

The currency-converter API from MCP360 — 1 operation(s) for currency-converter.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- currency-converter

#### Properties

- [OpenAPI](openapi/mcp360-currency-converter-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-currency-converter-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-currency-converter-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Dns Lookup API

The dns-lookup API from MCP360 — 2 operation(s) for dns-lookup.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- dns-lookup

#### Properties

- [OpenAPI](openapi/mcp360-dns-lookup-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-dns-lookup-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-dns-lookup-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Duckduckgo Search API

The duckduckgo-search API from MCP360 — 1 operation(s) for duckduckgo-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- duckduckgo-search

#### Properties

- [OpenAPI](openapi/mcp360-duckduckgo-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-duckduckgo-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-duckduckgo-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Ebay Search API

The ebay-search API from MCP360 — 3 operation(s) for ebay-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- ebay-search

#### Properties

- [OpenAPI](openapi/mcp360-ebay-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-ebay-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-ebay-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Email Verification API

The email-verification API from MCP360 — 2 operation(s) for email-verification.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- email-verification

#### Properties

- [OpenAPI](openapi/mcp360-email-verification-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-email-verification-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-email-verification-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Flights API

The google-flights API from MCP360 — 3 operation(s) for google-flights.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-flights

#### Properties

- [OpenAPI](openapi/mcp360-google-flights-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-flights-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-flights-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Forums API

The google-forums API from MCP360 — 1 operation(s) for google-forums.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-forums

#### Properties

- [OpenAPI](openapi/mcp360-google-forums-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-forums-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-forums-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Hotels API

The google-hotels API from MCP360 — 1 operation(s) for google-hotels.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-hotels

#### Properties

- [OpenAPI](openapi/mcp360-google-hotels-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-hotels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-hotels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Images API

The google-images API from MCP360 — 1 operation(s) for google-images.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-images

#### Properties

- [OpenAPI](openapi/mcp360-google-images-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-images-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-images-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Jobs API

The google-jobs API from MCP360 — 1 operation(s) for google-jobs.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-jobs

#### Properties

- [OpenAPI](openapi/mcp360-google-jobs-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-jobs-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-jobs-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Maps API

The google-maps API from MCP360 — 4 operation(s) for google-maps.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-maps

#### Properties

- [OpenAPI](openapi/mcp360-google-maps-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-maps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-maps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google News API

The google-news API from MCP360 — 2 operation(s) for google-news.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-news

#### Properties

- [OpenAPI](openapi/mcp360-google-news-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-news-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-news-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Play API

The google-play API from MCP360 — 2 operation(s) for google-play.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-play

#### Properties

- [OpenAPI](openapi/mcp360-google-play-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-play-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-play-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Rank Tracking API

The google-rank-tracking API from MCP360 — 3 operation(s) for google-rank-tracking.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-rank-tracking

#### Properties

- [OpenAPI](openapi/mcp360-google-rank-tracking-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-rank-tracking-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-rank-tracking-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Scholar API

The google-scholar API from MCP360 — 4 operation(s) for google-scholar.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-scholar

#### Properties

- [OpenAPI](openapi/mcp360-google-scholar-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-scholar-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-scholar-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Search API

The google-search API from MCP360 — 4 operation(s) for google-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-search

#### Properties

- [OpenAPI](openapi/mcp360-google-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Shopping API

The google-shopping API from MCP360 — 4 operation(s) for google-shopping.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-shopping

#### Properties

- [OpenAPI](openapi/mcp360-google-shopping-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-shopping-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-shopping-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Google Trends API

The google-trends API from MCP360 — 3 operation(s) for google-trends.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- google-trends

#### Properties

- [OpenAPI](openapi/mcp360-google-trends-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-google-trends-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-google-trends-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Imginny API

The imginny API from MCP360 — 4 operation(s) for imginny.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- imginny

#### Properties

- [OpenAPI](openapi/mcp360-imginny-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-imginny-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-imginny-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Ip Info API

The ip-info API from MCP360 — 2 operation(s) for ip-info.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- ip-info

#### Properties

- [OpenAPI](openapi/mcp360-ip-info-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-ip-info-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-ip-info-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Keyword Research API

The keyword-research API from MCP360 — 3 operation(s) for keyword-research.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- keyword-research

#### Properties

- [OpenAPI](openapi/mcp360-keyword-research-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-keyword-research-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-keyword-research-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Llm Prompt Tracker API

The llm-prompt-tracker API from MCP360 — 2 operation(s) for llm-prompt-tracker.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- llm-prompt-tracker

#### Properties

- [OpenAPI](openapi/mcp360-llm-prompt-tracker-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-llm-prompt-tracker-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-llm-prompt-tracker-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Mcp360 API

The mcp360 API from MCP360 — 2 operation(s) for mcp360.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- mcp360

#### Properties

- [OpenAPI](openapi/mcp360-mcp360-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-mcp360-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-mcp360-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Naver Search API

The naver-search API from MCP360 — 3 operation(s) for naver-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- naver-search

#### Properties

- [OpenAPI](openapi/mcp360-naver-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-naver-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-naver-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Onpage Seo API

The onpage-seo API from MCP360 — 2 operation(s) for onpage-seo.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- onpage-seo

#### Properties

- [OpenAPI](openapi/mcp360-onpage-seo-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-onpage-seo-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-onpage-seo-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 URL Lookup API

The url-lookup API from MCP360 — 2 operation(s) for url-lookup.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- url-lookup

#### Properties

- [OpenAPI](openapi/mcp360-url-lookup-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-url-lookup-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-url-lookup-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Walmart Search API

The walmart-search API from MCP360 — 2 operation(s) for walmart-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- walmart-search

#### Properties

- [OpenAPI](openapi/mcp360-walmart-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-walmart-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-walmart-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Weather API

The weather API from MCP360 — 3 operation(s) for weather.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- weather

#### Properties

- [OpenAPI](openapi/mcp360-weather-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-weather-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-weather-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Web Scraping API

The web-scraping API from MCP360 — 1 operation(s) for web-scraping.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- web-scraping

#### Properties

- [OpenAPI](openapi/mcp360-web-scraping-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-web-scraping-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-web-scraping-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Whois API

The whois API from MCP360 — 3 operation(s) for whois.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- whois

#### Properties

- [OpenAPI](openapi/mcp360-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Yahoo Search API

The yahoo-search API from MCP360 — 3 operation(s) for yahoo-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- yahoo-search

#### Properties

- [OpenAPI](openapi/mcp360-yahoo-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-yahoo-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-yahoo-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Yandex Search API

The yandex-search API from MCP360 — 3 operation(s) for yandex-search.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- yandex-search

#### Properties

- [OpenAPI](openapi/mcp360-yandex-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-yandex-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-yandex-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

### MCP360 Youtube API

The youtube API from MCP360 — 10 operation(s) for youtube.

- **Human URL:** [https://mcp360.ai/docs](https://mcp360.ai/docs)
- **Base URL:** `https://connect.mcp360.ai/api/v1`

#### Tags

- youtube

#### Properties

- [OpenAPI](openapi/mcp360-youtube-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mcp360-youtube-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mcp360-youtube-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P](https://connect.mcp360.ai/v1/mcp360/mcp)
- [Tool Crosswalk](mcp/mcp360-tool-crosswalk.yml)
- [JSON Schema](json-schema/mcp360-tool-schemas.json) — [JSON Schema](https://json-schema.org/specification)
- [L L M S Txt](https://mcp360.ai/llms.txt)
- [L L Ms Txt](llms/mcp360-llms.txt)
- [Documentation](https://mcp360.ai/docs)

## Common Properties

- [M C P Server](mcp/mcp360-mcp.yml)
- [Overlay](overlays/mcp360-amazon-search-overlay.yaml)
- [Developer Portal](https://dashboard.mcp360.ai)
- [Documentation](https://mcp360.ai/docs)
- [Getting Started](https://mcp360.ai/docs)
- [Help Center](https://help.mcp360.ai)
- [Support](https://mcp360.ai/contact)
- [Blog](https://mcp360.ai/blog)
- [GitHub Organization](https://github.com/mcp360)
- [Pricing](https://mcp360.ai/pricing)
- [Sign Up](https://dashboard.mcp360.ai/signup)
- [Login](https://dashboard.mcp360.ai/login)
- [Terms of Service](https://mcp360.ai/terms)
- [Privacy Policy](https://mcp360.ai/privacy)
- [Refund Policy](https://mcp360.ai/refund-policy)
- [Console](https://mcp360.ai/tools/mcp-inspector)
- [Authentication](authentication/mcp360-authentication.yml)
- [O Auth Scopes](scopes/mcp360-scopes.yml)
- [Well Known](well-known/mcp360-well-known.yml)
- [Conventions](conventions/mcp360-conventions.yml)
- [Error Catalog](errors/mcp360-problem-types.yml)
- [Lifecycle](lifecycle/mcp360-lifecycle.yml)
- [Conformance](conformance/mcp360-conformance.yml)
- [Data Model](data-model/mcp360-data-model.yml)
- [Packages](packages/mcp360-packages.yml)
- [S D Ks](packages/mcp360-packages.yml)
- [Plans](plans/mcp360-plans.yml)
- [Domain Security](security/mcp360-domain-security.yml)
- [Vulnerability Disclosure](security/mcp360-vulnerability-disclosure.yml)
- [Security](https://github.com/mcp360/mTarsier/blob/HEAD/SECURITY.md)
- [Agentic Access](agentic-access/mcp360-agentic-access.yml)
- [Agent Skill](skills/_index.yml)
- [Agent Skill](skills/mcp360-discover-and-execute-a-tool.md)
- [Agent Skill](skills/mcp360-run-a-web-search.md)
- [Agent Skill](skills/mcp360-profile-a-domain.md)
- [Agent Skill](skills/mcp360-audit-seo.md)
- [Agent Skill](skills/mcp360-compare-retail-prices.md)
- [Agent Skill](skills/mcp360-scrape-a-page.md)

## Maintainers

**FN:** Delta4 Infotech Pvt. Ltd.
**Email:** support@mcp360.ai
**URL:** https://mcp360.ai
