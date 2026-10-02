# Small Business Succession by State: Age of Employer-Business Owners (Census ABS)

Share of employer-business owners aged 55-64 and 65+, plus family ownership, prior-business outcomes and firm/payroll context, for 50 states + DC and the U.S., from the Census Bureau Annual Business Survey (data year 2023).

**Live page:** https://familyestateguide.com/estate-planning-data/small-business-succession-by-state/  
**Publisher:** Family Estate Guide (https://familyestateguide.com)  
**Version:** 1.0.0 (2026-10-02)  
**License:** CC BY 4.0 (data). See LICENSE.

> Not legal, tax, financial or medical advice. Figures are estimates with sampling error; legal rules change. Verify anything important with the original source or a qualified professional.

## Files

| File | Rows | Contents |
|---|---|---|
| `data/small-business-succession-by-state.csv` | 52 | 52 rows (50 states + DC + US). |

Blank cells mean not available, not published or not applicable; they are never zero.

## Data dictionary

### `data/small-business-succession-by-state.csv`

| Column | Description |
|---|---|
| `state` | State name (50 states + District of Columbia; some files add a United States row). |
| `abbr` | Two-letter USPS state abbreviation (US = national row). |
| `owners_reporting_age` | Owners of employer firms who reported their age (ABS counts up to 4 owners per firm). |
| `owners_55_64` | Owners aged 55-64. |
| `owners_65_plus` | Owners aged 65 or over. |
| `pct_owners_55_64` | Owners 55-64 as % of owners reporting age (ABS OWNPDEMP_PCT). |
| `pct_owners_65_plus` | Owners 65+ as % of owners reporting age. |
| `pct_owners_55_plus` | pct_owners_55_64 + pct_owners_65_plus. |
| `owners_55_plus` | owners_55_64 + owners_65_plus. |
| `rse_pct_owners_65_plus` | Relative standard error of the owners-65+ count, percent (ABS OWNPDEMP_S). |
| `se_pct_65_plus_pts` | Standard error of pct_owners_65_plus, percentage points (OWNPDEMP_PCT_S). |
| `employer_firms` | Number of employer firms (ABS company summary; all sizes). |
| `employees` | Number of employees (ABS company summary). |
| `annual_payroll_usd_thousands` | Annual payroll, thousands of USD. |
| `receipts_usd_thousands` | Sales, value of shipments or revenue, thousands of USD. |
| `pct_family_owned_of_reporting` | Family-owned firms as % of firms answering the family-ownership question. |
| `pct_owners_first_business` | Share of all owners for whom this is their first business, %. |
| `pct_owners_prior_biz_closed` | Share of all owners whose prior business is no longer in operation, %. |
| `pct_owners_prior_biz_sold` | Share of all owners whose prior business was purchased by another company or individual, %. |
| `pct_business_primary_income` | Share of owners for whom the business was their primary source of personal income, %. |

## Sources

- U.S. Census Bureau, Annual Business Survey (ABS), data year 2023: company summary (abscs), characteristics of business owners (abscbo) and characteristics of businesses (abscb), via https://api.census.gov/data/2023/ . Public domain.

## Methodology

- Owner age from abscbo QDESC OWNRAGE (owners of employer firms, percent of owners reporting). Firm counts and payroll from abscs. Family ownership from abscb.

## Limitations

- ABS counts owners (up to four per firm), not firms; the data cannot say how many firms will close.
- Firm, employee and payroll counts cover all employer firms, including large ones; they are context, not 'small business' totals.
- The 65+ share has RSE above 10% in AK, ND, SD and VT.
- Prior-business shares are of all current owners, not only owners with a prior business.
- No industry detail (sector-level owner-age queries returned no data).

## Rights review and exclusions

Family Estate Guide publishes here only its own compiled data and U.S. government public-domain data (Census, BLS, CMS, DOL), plus third-party data that is under CC BY or a compatible open license, with attribution. Third-party copyrighted or non-commercial-licensed data is excluded.

- Excluded U.S. Bank 'Small Business Perspective' (2025) and JPMorgan Chase Local Snapshot Succession Survey (2026) statistics (e.g., 54% with a formal plan, 8% fully prepared). They are quoted on the live page but are copyrighted, bank-sponsored surveys with no open license; they were never in the CSV and are not in this repo.

## How to cite

Family Estate Guide (2026). *Small Business Succession by State: Age of Employer-Business Owners (Census ABS)* (Version 1.0.0) [Data set]. https://familyestateguide.com/estate-planning-data/small-business-succession-by-state/ . GitHub: https://github.com/jameyriley46-ux/familyestateguide-small-business-succession-by-state

A Zenodo DOI will be added here once version 1.0.0 is released and archived. Machine-readable citation: `CITATION.cff`.

Please link to the live page when you use the data.

## License

Data in this repository is licensed under the Creative Commons Attribution 4.0 International license (CC BY 4.0). Underlying U.S. government data is public domain; third-party CC BY data keeps its original attribution requirements (see Sources).
