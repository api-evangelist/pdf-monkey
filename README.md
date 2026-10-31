# PDF Monkey

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

PDF Monkey is a PDF generation REST API that uses Handlebars templates to produce high-quality PDFs from JSON data. Developers build templates in a visual dashboard, call the API with dynamic JSON payloads, and retrieve generated documents via signed download URLs or webhooks. The service supports document management, asynchronous and synchronous generation, webhook notifications powered by Svix, fillable PDF forms, password protection, and integrations with Zapier, Make, and n8n.

**Areas:** PDF · Document Generation · Templates · Handlebars · REST API · Webhook

## PDF Monkey on APIs.io

Everything profiled for PDF Monkey is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/pdf-monkey/](https://apis.io/providers/pdf-monkey/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [PDF Monkey Authentication API](https://apis.io/apis/pdf-monkey/pdf-monkey-authentication-api/) — Endpoints for verifying API credentials and retrieving account information
- [PDF Monkey Documents API](https://apis.io/apis/pdf-monkey/pdf-monkey-documents-api/) — Create, retrieve, update, delete, and list PDF documents
- [PDF Monkey Templates API](https://apis.io/apis/pdf-monkey/pdf-monkey-templates-api/) — Manage document templates for PDF generation

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Pdf Monkey Agentic Access](https://apis.io/agentic-access/pdf-monkey/pdf-monkey-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Document](https://apis.io/schemas/pdf-monkey/document/)
- [DocumentTemplate](https://apis.io/schemas/pdf-monkey/document-template/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Pdf Monkey Context](https://apis.io/jsonld/pdf-monkey/pdf-monkey/)

#### Examples (3)

Example requests and responses.

- [Create Document](https://apis.io/examples/pdf-monkey/create-document/)
- [Create Document Sync](https://apis.io/examples/pdf-monkey/create-document-sync/)
- [List Documents](https://apis.io/examples/pdf-monkey/list-documents/)

#### Collections (5)

Postman and Open Collection request collections.

- [PDF Monkey Authentication API](https://apis.io/collections/pdf-monkey/open-pdf-monkey-authentication-api/)
- [PDFMonkey Document Cards API](https://apis.io/collections/pdf-monkey/open-pdf-monkey-document-cards-api/)
- [PDF Monkey Authentication Documents API](https://apis.io/collections/pdf-monkey/open-pdf-monkey-documents-api/)
- [PDF Monkey Authentication Templates API](https://apis.io/collections/pdf-monkey/open-pdf-monkey-templates-api/)
- [PDFMonkey API](https://apis.io/collections/pdf-monkey/open-pdfmonkey/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [PDF Monkey — jsonschema rules](https://apis.io/rules/pdf-monkey/pdf-monkey-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Pdf Monkey Authentication](https://apis.io/security/pdf-monkey/pdf-monkey-authentication/)
- [Pdf Monkey Domain Security](https://apis.io/security/pdf-monkey/pdf-monkey-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Pdf Monkey Plans Pricing](https://apis.io/plans/pdf-monkey/pdf-monkey-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Pdf Monkey Rate Limits](https://apis.io/rate-limits/pdf-monkey/pdf-monkey-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Pdf Monkey Finops](https://apis.io/finops/pdf-monkey/pdf-monkey-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.pdfmonkey.io)
- [Documentation](https://pdfmonkey.io/docs/)
- [Pricing](https://www.pdfmonkey.io/pricing/)
- [Blog](https://www.pdfmonkey.io/blog/)
- [GitHub](https://github.com/pdfmonkey)
- [Status](https://status.pdfmonkey.io/)

## API Evangelist rating

**Kin Score 32.8** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 62.6 |
| Contract governance | 9.8 |
| Operational transparency | 10.5 |
| Developer ergonomics | 23.8 |
| Access clarity | 18.4 |

**Agent readiness 22.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/pdf-monkey/](https://apis.io/providers/pdf-monkey/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for PDF Monkey: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/pdf-monkey/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
