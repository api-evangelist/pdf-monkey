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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

PDF Monkey is a PDF generation REST API that uses Handlebars templates to produce high-quality PDFs from JSON data. Developers build templates in a visual dashboard, call the API with dynamic JSON payloads, and retrieve generated documents via signed download URLs or webhooks.

## API

**Base URL:** `https://api.pdfmonkey.io/api/v1`

**Authentication:** Bearer token in the `Authorization` header. Obtain your secret key from the PDF Monkey dashboard.

### Key Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/documents` | Create and queue a document for async generation |
| POST | `/documents/sync` | Create a document and wait for completion (6-min timeout) |
| GET | `/document_cards/{id}` | Retrieve lightweight document status (recommended for polling) |
| GET | `/documents/{id}` | Retrieve full document with payload and logs |
| GET | `/document_cards` | List documents with pagination (24 per page) |
| PUT | `/documents/{id}` | Update document payload or trigger generation |
| DELETE | `/documents/{id}` | Permanently delete a document and its file |

### Webhooks

PDF Monkey uses Svix to deliver signed webhook notifications. Two event types are supported:

- `documents.generation.success` — document generated; `download_url` is available (valid 1 hour)
- `documents.generation.failure` — generation failed; `failure_cause` describes the error

Webhooks can be routed workspace-wide, per template, per folder, or per document via the `_webhook_channel` meta key.

## Plans

| Plan | Price (EUR/mo) | Documents/mo | Retention |
|------|---------------|--------------|-----------|
| Free | €0 | 20 | 1 day |
| Starter | €5 | 300 | 1 day |
| Pro | €15 | 3,000 | 7 days |
| Pro+ | €60 | 5,000 | Unlimited |
| Premium | €300 | 60,000 | Unlimited |

Annual billing saves 10%. Boost Packs add 1,000 documents for €5 each.

## Links

- **Website:** https://www.pdfmonkey.io
- **Documentation:** https://pdfmonkey.io/docs/
- **GitHub:** https://github.com/pdfmonkey
- **Status:** https://status.pdfmonkey.io/
- **Pricing:** https://www.pdfmonkey.io/pricing/
- **Blog:** https://www.pdfmonkey.io/blog/
- **LinkedIn:** https://www.linkedin.com/company/pdfmonkey/
- **X/Twitter:** https://twitter.com/pdfmonkey

## SDKs and Integrations

- **Ruby Gem:** [pdfmonkey-ruby](https://github.com/pdfmonkey/pdfmonkey-ruby)
- **CLI:** [pdfmonkey-cli](https://github.com/pdfmonkey/pdfmonkey-cli)
- **n8n:** [n8n-nodes-pdfmonkey](https://github.com/pdfmonkey/n8n-nodes-pdfmonkey)
- **Zapier:** [pdfmonkey-zapier](https://github.com/pdfmonkey/pdfmonkey-zapier)
- **Bubble:** [pdfmonkey-bubble](https://github.com/pdfmonkey/pdfmonkey-bubble)

## APIs.json

This repository contains an [APIs.json 0.19](https://apisjson.org) profile for PDF Monkey maintained by [API Evangelist](https://apievangelist.com).
