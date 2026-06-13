# PDF Monkey

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
