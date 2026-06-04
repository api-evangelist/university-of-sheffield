# University of Sheffield (university-of-sheffield)

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
