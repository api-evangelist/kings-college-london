# King's College London (kings-college-london)

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

King's College London (KCL) is a public research university in London, United Kingdom, ranked #41 in the QS World University Rankings 2025. King's does not operate a centralized public developer portal; its verifiable, machine-readable footprint lives in research and library infrastructure — the King's Research Portal (Pure) OAI-PMH interface and the King's research data repository hosted on Figshare. This repository catalogs that footprint as an APIs.json profile.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kings-college-london-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, OAI-PMH, Library, United Kingdom

## APIs

- **King's Research Portal (Pure) OAI-PMH** — OAI-PMH metadata harvesting interface for the King's Research Portal (Pure institutional repository). Base URL: `https://kclpure.kcl.ac.uk/ws/oai`. Docs: https://www.kcl.ac.uk/research/explore/kings-research-portal
- **King's College London Research Repository (Figshare)** — King's research data repository on Figshare, accessible via the Figshare public REST API and OAI-PMH endpoint. Base URL: `https://api.figshare.com/v2`. Docs: https://docs.figshare.com/ — Repository: https://kcl.figshare.com/

## Plans / Rate Limits / FinOps

- Plans: [plans/kings-college-london-plans-pricing.yml](plans/kings-college-london-plans-pricing.yml)
- Rate Limits: [rate-limits/kings-college-london-rate-limits.yml](rate-limits/kings-college-london-rate-limits.yml)
- FinOps: [finops/kings-college-london-finops.yml](finops/kings-college-london-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.kcl.ac.uk/
- GitHub: https://github.com/kcl-eresearch
- LinkedIn: https://www.linkedin.com/school/king's-college-london/
- Developer Portal (e-Research): https://docs.er.kcl.ac.uk/
- Review: [review.yml](review.yml)

## Notes

All cataloged APIs were verified against live endpoints in June 2026. The Pure OAI-PMH interface returned a valid `Identify` response (repositoryName "Pure OAI Repository"); the Figshare REST API and OAI-PMH endpoints both returned HTTP 200. The legacy `/ws/OAIHandler` path returned 405 — the canonical path is `/ws/oai`. The King's e-Research documentation portal (docs.er.kcl.ac.uk) and GitHub org (kcl-eresearch) are real but largely cover gated research-computing tools rather than open public APIs. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
