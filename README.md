# Inception

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

Inception Labs builds diffusion-based large language models (dLLMs) branded Mercury. Unlike autoregressive models that emit tokens one at a time, Mercury generates many tokens in parallel through discrete diffusion, running 5-10x faster at roughly half the cost of comparable frontier models. The Inception API is OpenAI-compatible and exposes chat completions (Mercury 2, a reasoning dLLM with a 128K context, tool calling, and structured outputs), plus fill-in-the-middle and next-edit code completions (Mercury Edit 2) for IDE-style autocomplete. It ships official Python and TypeScript SDKs, a streaming/diffusion mode, and enterprise deployment via the Inception API, AWS Bedrock, and Azure AI Foundry. Backed by Amplify Partners.

**Areas:** Company · Artificial Intelligence · LLM · Diffusion Models · Code Completion · Machine Learning · Developer Tools · Foundation Models

## Inception on APIs.io

Everything profiled for Inception is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/inception/](https://apis.io/providers/inception/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Inception Edit API](https://apis.io/apis/inception/inception-edit-api/) — Code edit completion endpoints.
- [Inception FIM API](https://apis.io/apis/inception/inception-fim-api/) — Fill-in-the-middle code completion endpoints.
- [Inception Models API](https://apis.io/apis/inception/inception-models-api/) — List available models.
- [Inception Chat Completions API](https://apis.io/apis/inception/inception-chat-completions-api/) — Chat completion endpoints (OpenAI-compatible).

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (2)

Multi-step workflows that chain operations into a business task.

- [Inception — discover a chat model and generate a completion](https://apis.io/arazzos/inception/inception-chat-completion.arazzo/)
- [Inception — fill-in-the-middle code autocomplete](https://apis.io/arazzos/inception/inception-code-autocomplete.arazzo/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [inception](https://apis.io/servers/inception/inception/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Inception Agentic Access](https://apis.io/agentic-access/inception/inception-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [Inception Chat API](https://apis.io/collections/inception/open-inception-chat-api/)
- [Inception Chat Edit API](https://apis.io/collections/inception/open-inception-edit-api/)
- [Inception Chat FIM API](https://apis.io/collections/inception/open-inception-fim-api/)
- [Inception Chat Models API](https://apis.io/collections/inception/open-inception-models-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Inception Openapi Overlay](https://apis.io/overlays/inception/inception-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Inception Authentication](https://apis.io/security/inception/inception-authentication/)
- [Inception Domain Security](https://apis.io/security/inception/inception-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Inception Plans](https://apis.io/plans/inception/inception-plans/)

#### Rate limits (1)

Published request limits.

- [Inception Rate Limits](https://apis.io/rate-limits/inception/inception-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Inception Finops](https://apis.io/finops/inception/inception-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://inceptionlabs.ai)
- [Documentation](https://docs.inceptionlabs.ai/get-started/get-started)
- [Getting started](https://docs.inceptionlabs.ai/get-started/get-started)
- [API reference](https://docs.inceptionlabs.ai/api-reference/chat/create-a-chat-completion)
- [Pricing](https://docs.inceptionlabs.ai/get-started/models)
- [Sign up](https://platform.inceptionlabs.ai/auth/login)
- [Support](https://docs.inceptionlabs.ai/support/support)
- [Blog](https://www.inceptionlabs.ai/blog)
- [Terms of service](https://docs.inceptionlabs.ai/support/tou)
- [Privacy policy](https://docs.inceptionlabs.ai/support/privacy)
- [GitHub](https://github.com/inception-ai-inc)

## API Evangelist rating

**Kin Score 47.9** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 55.7 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 58.9 |
| Access clarity | 69.7 |

**Agent readiness 31.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.7** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/inception/](https://apis.io/providers/inception/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Inception: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/inception/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
