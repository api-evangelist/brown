# Brown University (brown)

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
