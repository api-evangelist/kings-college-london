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

King's College London (KCL) is a UK public research university and Russell Group member, founded in 1829, ranked #40 in the QS World University Rankings. This repository profiles King's programmable footprint as an APIs.json profile, re-profiled on **2026-08-19** under the API Evangelist university pipeline, which settles **who operates** a surface before crediting it to the institution.

**What changed on 2026-08-19.** The June 2026 profile credited King's with eleven API entries and ten OpenAPI contracts. Every one of them described `api.figshare.com/v2` — a single Figshare document that the same pass attributed to twenty-five different universities, split by tag into eleven apparent surfaces. Those contracts, and the collections, schemas, examples and agentic-access classifications derived from them, have been removed. Figshare's API scores against Figshare's own repository, not King's.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kings-college-london-api-evangelist&utm_content=repo

## Type

- Index / Consumer / Private — `x-type: university`, `x-category: Public Research University`

## Tags

University, Higher Education, Education, Russell Group, United Kingdom, London, Research, Research Computing, Artificial Intelligence, Institutional Repository, Identity Federation, OAI-PMH, Library

## Surfaces, by operator

### Institution-operated

- **King's e-Research AI Hub API** — `https://ai.create.kcl.ac.uk/api/v1`. King's own OpenAI-compatible LLM inference platform for researchers, students and staff: chat completions, image generation, streaming, RAG, agent workflows and MCP integrations, reachable by pointing an OpenAI client at a new base URL. Live and bearer-authenticated — `GET /api/v1/models` returns 401 with the OpenAI error envelope, and answers differently for a missing header than for an unknown key. Runs on King's own e-Research load balancer (`lbext-vip.er.kcl.ac.uk`). No OpenAPI is published; the API reference at `/docs` is behind Microsoft Entra ID. Docs: https://docs.er.kcl.ac.uk/CREATE/ai_hub/

### Tenant — King's data, a vendor's contract

- **King's Research Portal (Pure) OAI-PMH** — `https://kclpure.kcl.ac.uk/ws/oai`. Fully open OAI-PMH 2.0, six metadata prefixes including `uketd_dc`, sets back to 1972. `kclpure.kcl.ac.uk` CNAMEs to `kings.elsevierpure.com`; the implementation is Elsevier Pure's.
- **Research data repository (Figshare)** — https://kcl.figshare.com/ CNAMEs to `figshare.com`. King's holds the DataCite membership (provider `HCBR`, ROR `0220mzb33`, prefix `10.18742`, 1,118 DOIs); Figshare holds the contract.
- **UK Access Management Federation / eduGAIN identity provider** — entityID `https://kclidp.kcl.ac.uk/idp/shibboleth`, registered 2010, SIRTFI-certified, scope `kcl.ac.uk`. The SSO endpoints resolve to `login.openathens.net/saml/2/sso/kcl.ac.uk/c/ukfed` — OpenAthens runs the IdP.
- **LibrarySearch** — https://librarysearch.kcl.ac.uk/ CNAMEs to `kcl.primo.exlibrisgroup.com` (Ex Libris Primo, `vid=44KCL_INST`).
- **KEATS virtual learning environment** — https://keats.kcl.ac.uk/ CNAMEs to `kcl-vle.bloom.ulcc.ac.uk` (Moodle, hosted by ULCC/Cosector). Live web-service and LTI endpoints; no LTI 1.3 JWKS or OIDC discovery.

### Real but not reachable from the public internet

- **CREATE Cloud OpenStack API** — documented at https://docs.er.kcl.ac.uk/CREATE/cloud/openstack_api/, requires OpenVPN, an OpenStack application credential and the KCL e-Research root CA. `cloud.er.kcl.ac.uk` publishes no public DNS record.
- **KCL e-Research Authentication API** — https://github.com/kcl-eresearch/auth_api documents King's own REST surface for SSH keys, OpenVPN certificates and MFA approvals. Internal; no public base URL, no OpenAPI.

## Artifacts

- Conformance (education regime): [conformance/kings-college-london-education-standards.yml](conformance/kings-college-london-education-standards.yml)
- Authentication: [authentication/kings-college-london-authentication.yml](authentication/kings-college-london-authentication.yml)
- Errors: [errors/kings-college-london-problem-types.yml](errors/kings-college-london-problem-types.yml)
- Domain security: [security/kings-college-london-domain-security.yml](security/kings-college-london-domain-security.yml)
- Plans: [plans/kings-college-london-plans-pricing.yml](plans/kings-college-london-plans-pricing.yml)
- Rate Limits: [rate-limits/kings-college-london-rate-limits.yml](rate-limits/kings-college-london-rate-limits.yml)
- FinOps: [finops/kings-college-london-finops.yml](finops/kings-college-london-finops.yml)
- Review: [review.yml](review.yml)

No `openapi/` directory exists in this repository, and that is the correct state: King's publishes no machine-readable API contract for any surface it operates.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Common Properties

- Website: https://www.kcl.ac.uk/
- GitHub: https://github.com/kcl-eresearch
- LinkedIn: https://www.linkedin.com/school/king's-college-london/
- Developer Portal (e-Research): https://docs.er.kcl.ac.uk/
- AI Policy: https://www.kcl.ac.uk/about/strategy/learning-and-teaching/ai-guidance
- Terms: https://www.kcl.ac.uk/terms · Privacy: https://www.kcl.ac.uk/terms/privacy

## Notes

Every claim above was probed live on 2026-08-19; 40+ hosts and paths were checked and the full status table is in `apis.yml` under `x-coverage.evidence`. Confirmed absent: no DNS for `data.kcl.ac.uk`, `developer.kcl.ac.uk`, `courses.kcl.ac.uk`, `sis.kcl.ac.uk`, `idp.kcl.ac.uk` or `sso.kcl.ac.uk`; `api.kcl.ac.uk` resolves to 137.73.130.161 but accepts no TCP connection on port 80 or 443; `www.kcl.ac.uk/llms.txt` and `/.well-known/security.txt` both return 404. King's is not a Crossref member and exposes no ORCID iD on any machine-readable surface. No endpoints were fabricated and no vendor contract is credited to the institution.

## Maintainers

- Kin Lane — kin@apievangelist.com
