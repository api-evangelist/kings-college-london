# King's College London (kings-college-london)

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
