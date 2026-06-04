# Brown University (brown)

Brown University is a private Ivy League research university in Providence, Rhode Island, ranked #57 in the QS World University Rankings 2025. Its public developer and API footprint is centered on the Brown University Library, which operates the Brown Digital Repository (BDR) with a documented public REST/search API and a IIIF image/presentation service, alongside an InCommon-federated Shibboleth/SAML single sign-on service and an active GitHub organization.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=brown-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research, Library, Digital Repository, IIIF, United States

## APIs

- **Brown Digital Repository (BDR) API** — Public REST/search API for the Brown Digital Repository. Docs: https://repository.library.brown.edu/studio/api-docs/ — Base: https://repository.library.brown.edu/api/search/
- **Brown Digital Repository IIIF Service** — IIIF image/presentation service exposing manifests for BDR objects. Docs: https://iiif.io/guides/guides/repository.library.brown.edu/ — Base: https://repository.library.brown.edu/iiif/
- **Brown Shibboleth Single Sign-On (SAML)** — InCommon-federated Shibboleth SAML 2.0 identity provider. Docs: https://ithelp.brown.edu/kb/shibboleth-single-sign-on

## Plans / Rate Limits / FinOps

- Plans: [plans/brown-plans-pricing.yml](plans/brown-plans-pricing.yml)
- Rate Limits: [rate-limits/brown-rate-limits.yml](rate-limits/brown-rate-limits.yml)
- FinOps: [finops/brown-finops.yml](finops/brown-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.brown.edu
- GitHub: https://github.com/Brown-University-Library
- LinkedIn: https://www.linkedin.com/school/brown-university/
- Developer Portal: https://repository.library.brown.edu/studio/api-docs/
- Authentication: https://sso.brown.edu/idp/shibboleth
- Review: [review.yml](review.yml)

## Notes

All APIs were verified live on 2026-06-03: the BDR search API (`/api/search/`) and IIIF service (`/iiif/`) both returned HTTP 200, as did the BDR API docs page (behind a human-verification gate), the Shibboleth IdP, the official website, and the GitHub organization. The historical hackatbrown student API (`api.students.brown.edu`) is now defunct (HTTP 404) and is intentionally not cataloged as a live API. No endpoints were fabricated; Brown's SIS, course-catalog, and internal systems are gated behind Brown authentication and are not publicly documented APIs.

## Maintainers

- Kin Lane — kin@apievangelist.com
