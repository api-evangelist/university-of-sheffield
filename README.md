# University of Sheffield (university-of-sheffield)

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

The University of Sheffield is a public research university in Sheffield, United Kingdom, and a member of the Russell Group. This repository catalogs its public developer and API footprint as an APIs.json provider profile, with the **operator** of every surface settled before anything was saved.

Sheffield's programmable footprint is small and mostly indirect. There is no central developer portal, no API gateway, no self-service key issuance, and no documented course, timetable or student-information API. What the institution genuinely operates is one first-party research API — the **Sheffield Solar API**, which publishes its own OpenAPI 3.1 document and serves keyless PV_Live estimates of GB solar generation — and its own **Shibboleth SAML identity provider**. Everything else that looks like a Sheffield API is a vendor's contract running under Sheffield's name.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-sheffield-api-evangelist&utm_content=repo

## Type

- University / Public Research University / Producer / Public

## Tags

University, Higher Education, Education, United Kingdom, Russell Group, Research Data, Open Access, OAI-PMH, Identity Federation, Solar Energy, Energy Data, Research Computing

## APIs

Every entry carries an `x-operator`: `institution` means Sheffield runs the thing the contract describes; `tenant` means Sheffield's data on a vendor's platform, where the relationship is real but the engineering is not Sheffield's.

- **Sheffield Solar API** — `x-operator: institution`. Sheffield's own research API, built and run by the Sheffield Solar group in Physics and Astronomy. PV_Live (near-real-time and historical GB solar PV generation by GSP and PES region), PV_Live_EU (European NUTS regions) and PV_Forecast (day-ahead). PV_Live reads are keyless and answered 200 on probe; PV_Forecast returns 401 without a registered `X-User-Id` header. Publishes its own OpenAPI 3.1 at https://api.solar.sheffield.ac.uk/openapi.json — Docs: https://www.solar.sheffield.ac.uk/api/
- **University of Sheffield Shibboleth Identity Provider** — `x-operator: institution`. Live SAML 2.0 metadata, entityID `https://idp.shef.ac.uk/shibboleth`, served from Sheffield's own domain. Machine-readable, institution-operated by definition, and the access path through which affiliates reach every bought platform. Metadata: https://idp.shef.ac.uk/idp/shibboleth
- **ORDA — Online Research Data** — `x-operator: tenant`. Sheffield's research data repository on figshare. Sheffield's records and DataCite DOIs (provider `ooki`, client `bl.shef`); figshare's platform and API contract. No spec is saved here on purpose. Portal: https://orda.shef.ac.uk/
- **White Rose Research Online OAI-PMH** — `x-operator: tenant`. Shared open-access EPrints repository (Leeds, Sheffield, York). OAI-PMH 2.0, thirteen metadata formats including `oai_dc_orcid`. Endpoint: https://eprints.whiterose.ac.uk/cgi/oai2
- **White Rose eTheses Online OAI-PMH** — `x-operator: tenant`. Shared electronic theses EPrints repository. OAI-PMH 2.0. Endpoint: https://etheses.whiterose.ac.uk/cgi/oai2

## Domain standard conformance (Kin Score `education` regime)

Probed 2026-08-30, reward-only, evidence in `conformance/`:

| Standard | Conformant | Operator | Evidence |
|---|---|---|---|
| shibboleth | yes | institution | `EntityDescriptor@entityID` at https://idp.shef.ac.uk/idp/shibboleth |
| saml | yes | institution | SAML 2.0 SSO/SLO bindings in the same metadata |
| oai-pmh | yes | tenant | `Identify` 200 on both White Rose endpoints, protocolVersion 2.0 |
| orcid | yes | tenant | `oai_dc_orcid` in WRRO `ListMetadataFormats` |
| datacite | yes | tenant | DataCite provider `ooki`, client `bl.shef` |

Not found: scim, lti, oneroster, ed-fi, caliper, qti, crossref.

## Plans

- plans/university-of-sheffield-plans-pricing.yml

## Rate Limits

- rate-limits/university-of-sheffield-rate-limits.yml

## FinOps

- finops/university-of-sheffield-finops.yml

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.sheffield.ac.uk/
- API Reference: https://api.solar.sheffield.ac.uk/redoc
- Identity Federation: https://idp.shef.ac.uk/idp/shibboleth
- Research Repository: https://orda.shef.ac.uk/
- Library Catalog: https://find.shef.ac.uk/
- Research Computing: https://docs.hpc.shef.ac.uk/en/latest/
- GitHub: https://github.com/SheffieldUni
- SourceCode (RSE/IT): https://github.com/rcgsheffield · https://github.com/RSE-Sheffield · https://github.com/SheffieldSolar
- LinkedIn: https://www.linkedin.com/school/university-of-sheffield/
- Twitter: https://twitter.com/sheffielduni

## Attribution correction, 2026-08-30

This profile was rebuilt under the API Evangelist university pipeline. The 2026-06-03 profile had saved **figshare's own contract** under Sheffield's slug: `openapi/_original/university-of-sheffield-orda.yaml` declared `info.title: Figshare API`, `contact: Figshare Support` and `servers: [https://api.figshare.com/v2]`. It had been split into ten per-tag specs and registered as eleven `apis[]` entries — eleven times the apparent footprint, for one vendor document that eleven other universities in this cohort also ship.

Ten contracts, their figshare source document, and thirty-six derived artifacts (schemas, structures, examples, rulesets, vocabulary, JSON-LD context, Postman/OpenCollection collections, scopes, authentication and capability edges) were removed, because everything derived from a vendor contract inherits its provenance. The ORDA relationship was **kept** and relabelled `tenant` — it is a real institutional fact, and deleting it to avoid the misattribution would have been the opposite error.

**Expect this repository's Kin Score to fall.** It should. The old number was largely figshare's.

## Notes

Probed 2026-08-30. `api.sheffield.ac.uk`, `data.sheffield.ac.uk`, `shib.sheffield.ac.uk` and `sso.sheffield.ac.uk` do not resolve. `llms.txt` and `.well-known/security.txt` return 404 on the main site. ORDA's own OAI-PMH endpoint is live but returns a Cloudflare 202 bot challenge to scripted clients, so its `Identify` response could not be read — a block on us, not a gap in Sheffield. `/health/live` and `/health/ready` are declared in the Sheffield Solar OpenAPI but return an nginx 404 at the public edge; recorded as contract drift in `lifecycle/`. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
