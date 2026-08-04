# Regional Australia Bank (regional-australia-bank)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Regional Australia Bank is a customer-owned (mutual) authorised deposit-taking institution (ADI) headquartered in Armidale and Port Macquarie, New South Wales. Founded in 1969 as New England Staff Credit Union at the University of New England, it grew through successive credit-union mergers into Community Mutual Group and rebranded as Regional Australia Bank in 2016; it is currently completing a merger with Summerland Bank. As a mutual, its customers are its owners, and it serves more than 100,000 members across regional NSW. As an active ADI it is a designated data holder under Australia's Consumer Data Right (CDR / Open Banking).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/apis.yml)

## Tags

- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer-Owned
- Product Reference Data
- Mutual Bank

## Timestamps

- **Created:** 2026-07-20
- **Modified:** 2026-07-20

## APIs

### Regional Australia Bank CDR Product Reference Data API

Public, unauthenticated Consumer Data Right (CDR) Product Reference Data (PRD) API. Serves Regional Australia Bank's openly available banking product catalogue (Get Products and Get Product Detail) at the CDS base path `/cds-au/v1/banking/products`, conforming to the DSB Consumer Data Standards. Confirmed live (HTTP 200, `x-v: 3`) returning a `data.products` array of 25 products; no authentication or CDR accreditation is required for this product-reference surface.

- **Human URL:** [https://www.regionalaustraliabank.com.au/help-and-support/data-sharing](https://www.regionalaustraliabank.com.au/help-and-support/data-sharing)
- **Base URL:** `https://public-data.cdr.regaustbank.io/cds-au/v1/banking/products`

#### Tags

- CDR
- Open Banking
- Product Reference Data
- Banking Products
- Public

#### Properties

- [Documentation](https://www.regionalaustraliabank.com.au/help-and-support/data-sharing)
- [API Reference](https://consumerdatastandardsaustralia.github.io/standards/#banking-apis)
- [OpenAPI](openapi/regional-australia-bank-cds-banking-products-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Website](https://www.regionalaustraliabank.com.au/)
- [Documentation](https://www.regionalaustraliabank.com.au/help-and-support/data-sharing)
- [Support](https://www.regionalaustraliabank.com.au/help-and-support)
- [LinkedIn](https://www.linkedin.com/company/regional-australia-bank)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
