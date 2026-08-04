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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Sheffield is a public research university in Sheffield, United Kingdom, ranked #105 in the QS World University Rankings 2025. This repository catalogs its public developer and API footprint as an APIs.json provider profile. Sheffield's public API surface is concentrated in open research infrastructure — the ORDA research data repository (figshare) and the shared White Rose EPrints repositories — rather than a single unified developer portal.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-sheffield-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Access, OAI-PMH, United Kingdom

## APIs

- **ORDA Research Data Repository (figshare API)** — Sheffield's research data repository on figshare, accessible via the figshare REST API and an OAI-PMH endpoint. Docs: https://docs.figshare.com/ — Portal: https://orda.shef.ac.uk/
- **White Rose Research Online OAI-PMH** — Shared open-access EPrints repository (Leeds, Sheffield, York); OAI-PMH metadata harvesting. Docs: https://eprints.whiterose.ac.uk/information.html — Endpoint: https://eprints.whiterose.ac.uk/cgi/oai2
- **White Rose eTheses Online OAI-PMH** — Shared electronic theses EPrints repository; OAI-PMH metadata harvesting. Portal: https://etheses.whiterose.ac.uk/ — Endpoint: https://etheses.whiterose.ac.uk/cgi/oai2

## Plans

- plans/university-of-sheffield-plans-pricing.yml

## Rate Limits

- rate-limits/university-of-sheffield-rate-limits.yml

## FinOps

- finops/university-of-sheffield-finops.yml

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.sheffield.ac.uk/
- GitHub: https://github.com/SheffieldUni
- SourceCode (RSE/IT): https://github.com/rcgsheffield
- LinkedIn: https://www.linkedin.com/school/university-of-sheffield/
- Twitter: https://twitter.com/sheffielduni

## Notes

All endpoints listed were probed on 2026-06-03; see review.yml for HTTP status results. The ORDA portal and OAI endpoint sit behind a Cloudflare challenge (HTTP 202) but resolve in-browser; the figshare REST API and both White Rose OAI-PMH Identify responses were verified live. No course, timetable, or student-information APIs are publicly documented, and no Sheffield-branded developer portal was found; institutional APIs are platform-provided (figshare, EPrints). No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
