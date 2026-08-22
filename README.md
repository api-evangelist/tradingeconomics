# Trading Economics (tradingeconomics)

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

Trading Economics provides economic data for 196 countries - more than 20 million time series covering economic indicators like interest rates, inflation, GDP, and unemployment - alongside an economic calendar, proprietary macro forecasts, historical data, and live market quotes, all delivered through a single REST API and a WebSocket streaming service.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/apis.yml)

## Access Model

The API documentation at [docs.tradingeconomics.com](https://docs.tradingeconomics.com) is fully public, and official client libraries (Python, Node.js) are open on [GitHub](https://github.com/tradingeconomics), but calling the API requires a **paid subscription** - you get an API client key (key:secret) by subscribing to a plan at [developer.tradingeconomics.com](https://developer.tradingeconomics.com/). There is no free tier: the long-standing `guest:guest` sample-data account **has been discontinued** for the REST API (verified with a live request on 2026-07-11, which returned a guest-account-discontinued message pointing at the pricing page). Trial accounts are limited to 100,000 data points and 100 data requests. Third-party comparisons (June 2026) place Standard at $149/month and Professional at $299/month, billed yearly, with Enterprise custom-priced by features, request volume, and redistribution rights.

## Tags

- Economic Indicators
- Interest Rates
- Macroeconomics
- Financial Data
- Economic Calendar
- Forecasts
- Markets

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### Trading Economics Indicators API

Latest values for more than 15,000 economic indicator time series sourced directly from official statistics agencies and central banks - interest rates, inflation, GDP, unemployment, trade, and more - queryable by country, by indicator across all countries, by ticker, plus sovereign credit ratings.

- **Human URL:** [https://docs.tradingeconomics.com/indicators/snapshot/](https://docs.tradingeconomics.com/indicators/snapshot/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Economic Indicators
- Interest Rates
- Inflation
- GDP
- Credit Ratings

#### Properties

- [Documentation](https://docs.tradingeconomics.com/indicators/snapshot/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Economic Calendar API

Around 1,600 scheduled economic events per month across more than 150 countries - central bank rate decisions, CPI, GDP, and employment releases - with actual, previous, consensus forecast, and Trading Economics forecast values, filterable by country, date range, importance, and calendar ID.

- **Human URL:** [https://docs.tradingeconomics.com/economic_calendar/snapshot/](https://docs.tradingeconomics.com/economic_calendar/snapshot/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Economic Calendar
- Central Banks
- Interest Rate Decisions
- Releases

#### Properties

- [Documentation](https://docs.tradingeconomics.com/economic_calendar/snapshot/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Markets API

Current quotes for commodities, currencies, stock market indexes, cryptocurrencies, and government bond yields across maturities from 1M to 30Y, plus per-symbol quotes, daily and intraday historical prices, and market search.

- **Human URL:** [https://docs.tradingeconomics.com/markets/snapshot/](https://docs.tradingeconomics.com/markets/snapshot/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Markets
- Bonds
- Currencies
- Commodities
- Stock Indexes

#### Properties

- [Documentation](https://docs.tradingeconomics.com/markets/snapshot/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Forecasts API

Multi-quarter projections for economic indicators - including interest rates, inflation, and GDP - built with a proprietary global macro model and analyst expectations, queryable by country, indicator, country-and-indicator, or ticker, plus forecasts for market instruments.

- **Human URL:** [https://docs.tradingeconomics.com/forecasts/indicators/](https://docs.tradingeconomics.com/forecasts/indicators/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Forecasts
- Macroeconomics
- Interest Rates
- Projections

#### Properties

- [Documentation](https://docs.tradingeconomics.com/forecasts/indicators/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Historical API

Full historical time series behind every indicator - by country and indicator with optional date ranges, by ticker, plus latest-updates endpoints for syncing revisions - capped at 10,000 rows per request.

- **Human URL:** [https://docs.tradingeconomics.com/indicators/historical/](https://docs.tradingeconomics.com/indicators/historical/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Historical Data
- Time Series
- Economic Indicators

#### Properties

- [Documentation](https://docs.tradingeconomics.com/indicators/historical/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Financials API

Company fundamentals by financial category or stock symbol, plus earnings and revenue calendars, dividends, IPOs, stock splits, and sector listings for listed companies.

- **Human URL:** [https://docs.tradingeconomics.com/financials/snapshot/](https://docs.tradingeconomics.com/financials/snapshot/)
- **Base URL:** `https://api.tradingeconomics.com`

#### Tags

- Financials
- Earnings
- Company Fundamentals

#### Properties

- [Documentation](https://docs.tradingeconomics.com/financials/snapshot/)
- [OpenAPI](openapi/tradingeconomics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradingeconomics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradingeconomics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Trading Economics Streaming API

Persistent WebSocket connection at wss://stream.tradingeconomics.com delivering live market quote ticks by symbol and push notifications for economic calendar releases, news, and earnings via subscribe topics, authorized with API client credentials.

- **Human URL:** [https://docs.tradingeconomics.com/markets/streaming/](https://docs.tradingeconomics.com/markets/streaming/)
- **Base URL:** `wss://stream.tradingeconomics.com`

#### Tags

- Streaming
- WebSocket
- Real Time
- Economic Calendar
- Markets

#### Properties

- [Documentation](https://docs.tradingeconomics.com/markets/streaming/)
- [Documentation](https://docs.tradingeconomics.com/economic_calendar/streaming/)
- [AsyncAPI](asyncapi/tradingeconomics-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

## Common Properties

- [Website](https://tradingeconomics.com)
- [Documentation](https://docs.tradingeconomics.com)
- [GitHub Organization](https://github.com/tradingeconomics)
- [LinkedIn](https://www.linkedin.com/company/tradingeconomics)
- [Pricing](https://tradingeconomics.com/api/pricing.aspx)
- [Plans](plans/tradingeconomics-plans-pricing.yml)
- [Rate Limits](rate-limits/tradingeconomics-rate-limits.yml)
- [Fin Ops](finops/tradingeconomics-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
