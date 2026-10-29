# Brown University

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

Brown University is a private Ivy League research university in Providence, Rhode Island. Its genuinely institution-operated programmable footprint is narrow, real, and concentrated entirely in the Brown University Library. Three surfaces survive an operator check: the Brown Digital Repository (BDR) REST API, the BDR's IIIF Image and Presentation services, and a Shibboleth SAML 2.0 identity provider. All three sit under brown.edu, and the identity provider resolves into Brown's own ARIN allocation (BROWN-UNIV, 128.148.252.0/24) behind a Brown-procured InCommon OV certificate, so the attribution is settled by address ownership rather than by hostname. The BDR API is the substantive find: a public, keyless, Solr-backed API over 1,147,400 objects, documented by Brown Library staff in the wiki of Brown's own GitHub repository, with 11,622 objects exposing DataCite DOIs on Brown's prefix 10.26300. It is more than most universities in this cohort operate. It is also unversioned, sends no CORS headers, returns nine-byte text/html bodies on failure, silently caps results at 500 rows, and answers malformed queries with HTTP 200 and an empty result set rather than the 400 its own documentation promises. There is no OAI-PMH endpoint on any probed path — an absence worth stating, because reviewers assume an institutional repository has one. Everything else that looks like a Brown API is a vendor platform running under a Brown hostname and is recorded here as a tenant relationship, not as a Brown contract: library discovery is Ex Libris Primo VE (bruknow.library.brown.edu terminates on Ex Libris (USA) Inc address space), the course catalog and bulletin are Leepfrog CourseLeaf (cab.brown.edu and bulletin.brown.edu CNAME to courseleaf.com), and the events calendar is LiveWhale (events.brown.edu CNAMEs to lwcal.com). Two of those tenant platforms expose genuinely useful public JSON — Courses@Brown returns full section, meeting-time and instructor data with no key, and Events@Brown serves a 3MB JSON feed and an iCal feed — but that engineering is the vendor's. No central developer portal, no open data portal, and no institution-operated course or registrar API exist; the one that did, the student-built api.students.brown.edu, has been 404 since before this profile was first written.

**Areas:** Education · Higher Education · University · United States · Ivy League · Research · Research Repository · Digital Repository · Library · IIIF · Identity Federation · Course Catalog

## Brown University on APIs.io

Everything profiled for Brown University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/brown/](https://apis.io/providers/brown/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Brown University Identity Provider (Shibboleth / SAML 2.0)](https://apis.io/apis/brown/idp/) — Brown's Shibboleth identity provider, and the strongest machine-readable contract in this profile. Brown self-publishes signed per-entity SAML metadata at…
- [BruKnow Library Discovery (Ex Libris Primo VE tenant)](https://apis.io/apis/brown/bruknow/) — Brown University Library's discovery layer. search.library.brown.edu redirects to bruknow.library.brown.edu/discovery/search?vid=01BU_INST:BROWN, an Ex…
- [Courses@Brown (Leepfrog CourseLeaf tenant)](https://apis.io/apis/brown/cab/) — Brown's course search and registration front end. It exposes a live, public, keyless JSON API at cab.brown.edu/api/ — a POST interface with page=fose routes…
- [Brown University Bulletin (Leepfrog CourseLeaf CAT tenant)](https://apis.io/apis/brown/bulletin/) — The university's academic catalog of programs, concentrations and requirements, on the same vendor as Courses@Brown but a separate deployment.…
- [Events@Brown (LiveWhale Calendar tenant)](https://apis.io/apis/brown/events/) — Brown's university-wide events calendar, serving a public JSON feed at /live/json/events (3,128,496 bytes on 2026-08-30) and an iCalendar feed at…
- [Brown University Collections API](https://apis.io/apis/brown/brown-collections-api/) — Repository collections and their membership.
- [Brown University Discovery API](https://apis.io/apis/brown/brown-discovery-api/) — The API root link index.
- [Brown University IIIF Image API](https://apis.io/apis/brown/brown-iiif-image-api/) — IIIF Image API 2.x — image information and derivative delivery.
- [Brown University IIIF Presentation API](https://apis.io/apis/brown/brown-iiif-presentation-api/) — IIIF Presentation API 2.x — manifests describing an object's structure and metadata.
- [Brown University Items API](https://apis.io/apis/brown/brown-items-api/) — Metadata for a single repository object, addressed by PID.
- [Brown University Search API](https://apis.io/apis/brown/brown-search-api/) — Solr-backed search across public BDR objects.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (11)

The data models the API reads and writes.

- [ApiRoot](https://apis.io/schemas/brown/brown-bdr-apiroot/)
- [Collection](https://apis.io/schemas/brown/brown-bdr-collection/)
- [CollectionList](https://apis.io/schemas/brown/brown-bdr-collectionlist/)
- [CollectionRef](https://apis.io/schemas/brown/brown-bdr-collectionref/)
- [Document](https://apis.io/schemas/brown/brown-bdr-document/)
- [ImageInfo](https://apis.io/schemas/brown/brown-bdr-imageinfo/)
- [Item](https://apis.io/schemas/brown/brown-bdr-item/)
- [ItemLinks](https://apis.io/schemas/brown/brown-bdr-itemlinks/)
- [Manifest](https://apis.io/schemas/brown/brown-bdr-manifest/)
- [Relations](https://apis.io/schemas/brown/brown-bdr-relations/)
- [SearchResponse](https://apis.io/schemas/brown/brown-bdr-searchresponse/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Brown Context](https://apis.io/jsonld/brown/brown-context/)

#### Examples (7)

Example requests and responses.

- [Bdr Api Root](https://apis.io/examples/brown/bdr-api-root/)
- [Bdr Collections Top Level](https://apis.io/examples/brown/bdr-collections-top-level/)
- [Bdr Iiif Image Info](https://apis.io/examples/brown/bdr-iiif-image-info/)
- [Bdr Iiif Presentation Manifest](https://apis.io/examples/brown/bdr-iiif-presentation-manifest/)
- [Bdr Item](https://apis.io/examples/brown/bdr-item/)
- [Bdr Search Filtered](https://apis.io/examples/brown/bdr-search-filtered/)
- [Bdr Search Malformed Query](https://apis.io/examples/brown/bdr-search-malformed-query/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Brown University — bdr lint report rules](https://apis.io/rules/brown/brown-bdr-lint-report/)
- [Brown University — bdr rules](https://apis.io/rules/brown/brown-bdr-spectral-ruleset/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Brown Authentication](https://apis.io/security/brown/brown-authentication/)
- [Brown Domain Security](https://apis.io/security/brown/brown-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Brown Plans Pricing](https://apis.io/plans/brown/brown-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Brown Rate Limits](https://apis.io/rate-limits/brown/brown-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Brown Finops](https://apis.io/finops/brown/brown-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.brown.edu)
- [Documentation](https://github.com/Brown-University-Library/bdr_api_documentation/wiki)
- [API reference](https://repository.library.brown.edu/studio/api-docs/)
- [Support](https://ithelp.brown.edu/)
- [Blog](https://www.brown.edu/news)
- [Terms of service](https://policy.brown.edu/policy/acceptable-use-it-resources)
- [Privacy policy](https://policy.brown.edu/policy/privacy)
- [GitHub](https://github.com/Brown-University-Library)

## API Evangelist rating

**Kin Score 30.1** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 24.9 |
| Contract governance | 17.4 |
| Operational transparency | 10.5 |
| Developer ergonomics | 35.7 |
| Access clarity | 26.3 |

**Agent readiness 24.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 24.5** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/brown/](https://apis.io/providers/brown/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Brown University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/brown/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
