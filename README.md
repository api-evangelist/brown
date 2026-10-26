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

Brown University is a private Ivy League research university in Providence, Rhode Island. Its genuinely institution-operated programmable footprint is narrow, real, and concentrated entirely in the Brown University Library: the Brown Digital Repository (BDR) REST API, the BDR's IIIF Image and Presentation services, and a Shibboleth SAML 2.0 identity provider. Everything else that looks like a Brown API is a vendor platform running under a Brown hostname and is recorded here as a tenant relationship, not as a Brown contract.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=brown-api-evangelist&utm_content=repo

## Type

- Index
- university / Private Research University
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, United States, Ivy League, Research, Research Repository, Digital Repository, Library, IIIF, Identity Federation, Course Catalog, Research Computing

## Who operates what

Every surface carries an `x-operator`. `method:` says how we came to hold an artifact; `x-operator:` says who runs the thing it describes, and for a university those are rarely the same answer. Operator was settled by DNS CNAME and IP ownership, not by hostname — all seven hosts below are under `brown.edu`, and four of them are somebody else's infrastructure.

### Institution-operated — Brown's own

- **Brown Digital Repository (BDR) API** — `https://repository.library.brown.edu/api/` — public, keyless, Solr-backed, 1,147,400 objects. Item, collection and search endpoints. Brown University Library software, published open source in Brown's own GitHub org; registered with DataCite as client `BROWN.BDR` with 14,089 DOIs on prefix `10.26300`. Docs: https://github.com/Brown-University-Library/bdr_api_documentation/wiki
- **BDR IIIF Image and Presentation API** — `https://repository.library.brown.edu/iiif/` — IIIF Image API 2.x and Presentation API 2.x. Brown is a IIIF community case study.
- **Brown University Identity Provider** — `https://sso.brown.edu/idp/` — self-published, InCommon-registered SAML 2.0 / Shibboleth metadata. Resolves into `BROWN-UNIV` (ARIN) behind a Brown-subject InCommon OV certificate.

### Tenant — Brown's data, someone else's contract

- **BruKnow Library Discovery** — `bruknow.library.brown.edu` CNAMEs to `brown.primo.exlibrisgroup.com`; IP is Ex Libris (USA) Inc. Ex Libris Primo VE.
- **Courses@Brown** — `cab.brown.edu` CNAMEs to `brown-fs.courseleaf.com`. Leepfrog CourseLeaf. Serves a live keyless JSON course API; the engineering is the vendor's.
- **Brown University Bulletin** — `bulletin.brown.edu` CNAMEs to `brown-public.courseleaf.com`. CourseLeaf CAT.
- **Events@Brown** — `events.brown.edu` CNAMEs to `brown-prod.lwcal.com`. LiveWhale Calendar; JSON and iCal feeds.

## Contracts and artifacts

Brown publishes no OpenAPI. Both specifications here are **derived** — reconciled between Brown's own prose documentation and live probes on 2026-08-30 — and are marked as such in `info.x-provenance`. They are not Brown-authored contracts.

- OpenAPI: [openapi/brown-bdr-api-openapi.yml](openapi/brown-bdr-api-openapi.yml), [openapi/brown-bdr-iiif-openapi.yml](openapi/brown-bdr-iiif-openapi.yml) (pristine copies in [openapi/_original/](openapi/_original/))
- JSON Schema: [json-schema/](json-schema/) — 11 schemas
- Examples: [examples/](examples/) — 7 captured payloads
- Errors: [errors/brown-bdr-errors.yml](errors/brown-bdr-errors.yml)
- Vocabulary: [vocabulary/brown-bdr-field-vocabulary.yml](vocabulary/brown-bdr-field-vocabulary.yml)
- Rules: [rules/brown-bdr-spectral-ruleset.yml](rules/brown-bdr-spectral-ruleset.yml), [rules/brown-bdr-lint-report.yml](rules/brown-bdr-lint-report.yml)
- Authentication: [authentication/brown-authentication.yml](authentication/brown-authentication.yml)
- Lifecycle: [lifecycle/brown-lifecycle.yml](lifecycle/brown-lifecycle.yml)
- Conformance: [conformance/brown-conformance.yml](conformance/brown-conformance.yml)
- Identity Federation: [identity-federation/](identity-federation/) — analysis plus both SAML metadata documents

## Domain standards (Kin Score `education` regime)

Evidenced as institution-operated: **saml**, **shibboleth**, **datacite**. Partial and deliberately weak: crossref. Absent, and actively probed rather than assumed: **oai-pmh** (404 on seven candidate paths), **orcid** (zero matches index-wide). Not applicable or not found: scim, lti, oneroster, ed-fi, caliper, qti.

Also implemented, outside the regime list: IIIF Image 2.x, IIIF Presentation 2.x, MODS, Darwin Core (66,623 objects), FAST subject headings, Getty AAT.

## Plans / Rate Limits / FinOps

- Plans: [plans/brown-plans-pricing.yml](plans/brown-plans-pricing.yml)
- Rate Limits: [rate-limits/brown-rate-limits.yml](rate-limits/brown-rate-limits.yml)
- FinOps: [finops/brown-finops.yml](finops/brown-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.brown.edu
- GitHub: https://github.com/Brown-University-Library, https://github.com/brown-ccv
- Documentation: https://github.com/Brown-University-Library/bdr_api_documentation/wiki
- API Reference: https://repository.library.brown.edu/studio/api-docs/ (Cloudflare Turnstile interstitial for non-browser clients)
- Research Repository: https://repository.library.brown.edu/studio/
- Identity Federation: https://sso.brown.edu/idp/shibboleth
- Research Computing: https://ccv.brown.edu/
- AI Policy: https://provost.brown.edu/committees-and-reports/generative-ai-teaching-and-learning-gaitl-committee-charge
- Privacy Policy: https://policy.brown.edu/policy/privacy
- Terms of Service: https://policy.brown.edu/policy/acceptable-use-it-resources
- Support: https://ithelp.brown.edu/
- LinkedIn: https://www.linkedin.com/school/brown-university/
- Review: [review.yml](review.yml)

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline. Brown came through the vendor-attribution audit clean — no vendor contract had been misattributed to it, so nothing was removed. What the pass added is the contract work that was missing: two derived OpenAPIs, eleven JSON Schemas, seven captured payloads, and the errors, vocabulary, authentication, lifecycle, conformance and identity-federation artifacts.

Behaviours worth knowing before integrating, all probed rather than assumed: the search API silently clamps `rows` to 500; malformed queries return HTTP 200 with an empty result set rather than the documented 400; an unknown PID returns a nine-byte `text/html` "Not Found" rather than the documented 403 and not JSON; no CORS headers are sent, and JSONP via a `callback` parameter is the documented cross-origin path; and Cloudflare bot protection added in Spring 2025 fronts the host, serving a Turnstile interstitial on the human `/studio/` surface while leaving the JSON API open.

Named absences: no OAI-PMH endpoint, no open data portal, no `api.brown.edu`, no `developer.brown.edu`, no `llms.txt`, no `security.txt`, no OAuth or OIDC, and no institution-operated course or registrar API. The one that existed, the student-built `api.students.brown.edu`, has been 404 since before this profile was first written.

## Maintainers

- Kin Lane — kin@apievangelist.com
