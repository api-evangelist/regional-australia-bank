---
name: Browse Regional Australia Bank banking products
description: >-
  Retrieve and inspect Regional Australia Bank's openly offered banking products
  via the public, unauthenticated CDR Product Reference Data API. No credentials
  required; only the x-v version header.
api: openapi/regional-australia-bank-cds-banking-products-openapi.yml
operations:
  - listBankingProducts
  - getBankingProductDetail
---

# Browse Regional Australia Bank banking products

Regional Australia Bank exposes a **public, unauthenticated** Consumer Data Right
(CDR) Product Reference Data (PRD) API. Use it to list and inspect the bank's
openly offered products. No API key, OAuth token, or CDR accreditation is needed.

## Base URL

```
https://public-data.cdr.regaustbank.io/cds-au/v1
```

## Required header

Every request MUST include the endpoint version header:

```
x-v: 5
```

If the version is unsupported the API returns `406 Unsupported Version`. You may
also send `x-min-v` to accept a range.

## Steps

1. **List products** — call `listBankingProducts`:
   `GET /banking/products?effective=CURRENT&page=1&page-size=25`
   Optional filters: `effective` (ALL|CURRENT|FUTURE), `updated-since`,
   `brand`, `product-category` (e.g. `TRANS_AND_SAVINGS_ACCOUNTS`,
   `RESIDENTIAL_MORTGAGES`, `TERM_DEPOSITS`, `PERS_LOANS`, `CRED_AND_CHRG_CARDS`).
   Read `data.products[]` and paginate with `links`/`meta` (`page`, `page-size`).

2. **Get product detail** — for a chosen `productId` from step 1, call
   `getBankingProductDetail`: `GET /banking/products/{productId}` (send `x-v: 5`).
   Read fees, rates, features, eligibility, and constraints from `data`.

## Conventions

- **Pagination**: `page` / `page-size` (default 25); totals in `meta`.
- **Errors**: CDR `ResponseErrorListV2` envelope — an `errors[]` array of
  `{code, title, detail, meta}`. See `errors/regional-australia-bank-problem-types.yml`.
- **Idempotency**: not applicable — these are read-only GET operations.

## Scope boundary

Only these two product operations are public. Accounts, balances, transactions,
payees, and scheduled payments require CDR OAuth2/OIDC and accredited-data-recipient
registration — do not attempt them from an unaccredited client.
