# Agnost AI

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

Agnost AI is a production monitoring and product-analytics platform for teams building chat and voice AI agents. It continuously reads production agent conversations, MCP tool calls, and OpenTelemetry traces, clusters recurring intents, feature requests, frustration, and failure patterns, and catches agent failures that offline evals miss. It then turns the highest-impact patterns into reviewed fixes, including pull requests against prompts, tools, and agent harnesses. Agnost is OpenTelemetry-native, works with any LLM and framework, and ships SDKs for Python and TypeScript conversation tracking, MCP-server analytics (Python, TypeScript, Go), plus a hosted OAuth-protected MCP server for querying your dashboard from Claude Desktop, Cursor, and any MCP client. Founded in 2025 and part of Y Combinator's Summer 2026 (S26) batch.

**Areas:** Company · AI Agents · Agent Analytics · Observability · OpenTelemetry · MCP · Conversational AI · Monitoring · Developer Tools · Analytics

## Agnost AI on APIs.io

Everything profiled for Agnost AI is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/agnost-ai/](https://apis.io/providers/agnost-ai/)** — or go straight to one of the APIs or properties below.

### APIs (14)

- [Agnost AI Alerts API](https://apis.io/apis/agnost-ai/agnost-ai-alerts-api/) — Alert configuration and monitoring
- [Agnost AI API Keys API](https://apis.io/apis/agnost-ai/agnost-ai-api-keys-api/) — API key management
- [Agnost AI Auth API](https://apis.io/apis/agnost-ai/agnost-ai-auth-api/) — OAuth authentication callbacks
- [Agnost AI Billing API](https://apis.io/apis/agnost-ai/agnost-ai-billing-api/) — Stripe billing management
- [Agnost AI Classification API](https://apis.io/apis/agnost-ai/agnost-ai-classification-api/) — LLM-based classification operations
- [Agnost AI Connections API](https://apis.io/apis/agnost-ai/agnost-ai-connections-api/) — External integrations (Slack)
- [Agnost AI Conversations API](https://apis.io/apis/agnost-ai/agnost-ai-conversations-api/) — Conversation message and span retrieval
- [Agnost AI Dashboard API](https://apis.io/apis/agnost-ai/agnost-ai-dashboard-api/) — Analytics and metrics for the dashboard
- [Agnost AI Onboarding API](https://apis.io/apis/agnost-ai/agnost-ai-onboarding-api/) — First-run helpers used during organization setup
- [Agnost AI Organizations API](https://apis.io/apis/agnost-ai/agnost-ai-organizations-api/) — Organization management
- [Agnost AI SDK API](https://apis.io/apis/agnost-ai/agnost-ai-sdk-api/) — Event ingestion endpoints used by SDKs
- [Agnost AI Sentiments API](https://apis.io/apis/agnost-ai/agnost-ai-sentiments-api/) — Sentiment and intent analysis
- [Agnost AI SOPs API](https://apis.io/apis/agnost-ai/agnost-ai-sops-api/) — Standard Operating Procedures
- [Agnost AI System API](https://apis.io/apis/agnost-ai/agnost-ai-system-api/) — Health checks, webhooks, internal endpoints

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Agnost MCP Server](https://apis.io/servers/agnost-ai/agnost-mcp-server/)

#### Collections (14)

Postman and Open Collection request collections.

- [Agnost AI Alerts API](https://apis.io/collections/agnost-ai/open-agnost-ai-alerts-api/)
- [Agnost AI Alerts API Keys API](https://apis.io/collections/agnost-ai/open-agnost-ai-api-keys-api/)
- [Agnost AI Alerts Auth API](https://apis.io/collections/agnost-ai/open-agnost-ai-auth-api/)
- [Agnost AI Alerts Billing API](https://apis.io/collections/agnost-ai/open-agnost-ai-billing-api/)
- [Agnost AI Alerts Classification API](https://apis.io/collections/agnost-ai/open-agnost-ai-classification-api/)
- [Agnost AI Alerts Connections API](https://apis.io/collections/agnost-ai/open-agnost-ai-connections-api/)
- [Agnost AI Alerts Conversations API](https://apis.io/collections/agnost-ai/open-agnost-ai-conversations-api/)
- [Agnost AI Alerts Dashboard API](https://apis.io/collections/agnost-ai/open-agnost-ai-dashboard-api/)
- [Agnost AI Alerts Onboarding API](https://apis.io/collections/agnost-ai/open-agnost-ai-onboarding-api/)
- [Agnost AI Alerts Organizations API](https://apis.io/collections/agnost-ai/open-agnost-ai-organizations-api/)
- [Agnost AI Alerts SDK API](https://apis.io/collections/agnost-ai/open-agnost-ai-sdk-api/)
- [Agnost AI Alerts Sentiments API](https://apis.io/collections/agnost-ai/open-agnost-ai-sentiments-api/)
- [Agnost AI Alerts SOPs API](https://apis.io/collections/agnost-ai/open-agnost-ai-sops-api/)
- [Agnost AI Alerts System API](https://apis.io/collections/agnost-ai/open-agnost-ai-system-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Agnost Ai Openapi Overlay](https://apis.io/overlays/agnost-ai/agnost-ai-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Agnost Ai Authentication](https://apis.io/security/agnost-ai/agnost-ai-authentication/)
- [Agnost Ai Domain Security](https://apis.io/security/agnost-ai/agnost-ai-domain-security/)
- [Agnost Ai Trust Center](https://apis.io/security/agnost-ai/agnost-ai-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Agnost Ai Scopes](https://apis.io/scopes/agnost-ai/agnost-ai-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.agnost.ai/)
- [Documentation](https://docs.agnost.ai)
- [Getting started](https://docs.agnost.ai/quickstart)
- [API reference](https://docs.agnost.ai/openapi.yaml)
- [Pricing](https://agnost.ai/)
- [Sign up](https://app.agnost.ai)
- [Support](https://call.agnost.ai)
- [Blog](https://agnost.ai/blog/)
- [Compliance](https://trust.agnost.ai)
- [Terms of service](https://agnost.ai/terms)
- [GitHub](https://github.com/agnostai)
- [Status](https://status.agnost.ai)

## API Evangelist rating

**Kin Score 49.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 45.5 |
| Contract governance | 18.2 |
| Operational transparency | 26.3 |
| Developer ergonomics | 66.1 |
| Access clarity | 50.0 |

**Agent readiness 47.7** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/agnost-ai/](https://apis.io/providers/agnost-ai/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Agnost AI: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/agnost-ai/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
