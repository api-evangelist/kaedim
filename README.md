# Kaedim

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

Kaedim is an AI 3D asset generation company (backed by a16z) that turns 2D images — photos, sketches and concept art — into production-ready 3D models for games, e-commerce and simulation. The Enterprise Web API lets developers integrate Kaedim's 2D-to-3D pipeline into internal modelling workflows and user-generated-content products: submit up to six images at a chosen level of quality, track generation by requestID, receive results via signed webhooks, and download models in obj, fbx, glb, gltf, mtl and usd formats. Kaedim also ships first-party plugins for Unity, Unreal, Blender, Cinema 4D and NVIDIA Omniverse. Authentication uses an X-API-Key header plus a 12-hour JWT bearer token; generation is asynchronous and completes in roughly 10-15 minutes.

**Areas:** Company · 3D · Artificial Intelligence · Generative AI · Gaming · 3D Models · Asset Generation · Content Generation · Machine Learning

## Kaedim on APIs.io

Everything profiled for Kaedim is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kaedim/](https://apis.io/providers/kaedim/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Kaedim Assets API](https://apis.io/apis/kaedim/kaedim-assets-api/) — Fetch generated assets and projects
- [Kaedim Auth API](https://apis.io/apis/kaedim/kaedim-auth-api/) — Token refresh
- [Kaedim Generation API](https://apis.io/apis/kaedim/kaedim-generation-api/) — Submit images for 3D asset generation
- [Kaedim Webhooks API](https://apis.io/apis/kaedim/kaedim-webhooks-api/) — Register a webhook endpoint and obtain a JWT

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Kaedim Webhooks](https://apis.io/asyncapis/kaedim/kaedim-webhooks-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [{destination}](https://apis.io/channels/kaedim/destination/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [kaedim](https://apis.io/servers/kaedim/kaedim/)

#### Collections (4)

Postman and Open Collection request collections.

- [Kaedim Web Assets API](https://apis.io/collections/kaedim/open-kaedim-assets-api/)
- [Kaedim Web Assets Auth API](https://apis.io/collections/kaedim/open-kaedim-auth-api/)
- [Kaedim Web Assets Generation API](https://apis.io/collections/kaedim/open-kaedim-generation-api/)
- [Kaedim Web Assets Webhooks API](https://apis.io/collections/kaedim/open-kaedim-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Kaedim Web Api Overlay](https://apis.io/overlays/kaedim/kaedim-web-api-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Kaedim Authentication](https://apis.io/security/kaedim/kaedim-authentication/)
- [Kaedim Domain Security](https://apis.io/security/kaedim/kaedim-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Kaedim Plans Pricing](https://apis.io/plans/kaedim/kaedim-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kaedim3d.com)
- [Documentation](https://docs.kaedim3d.com)
- [Getting started](https://docs.kaedim3d.com/welcome/get-started/quick-start)
- [API reference](https://docs.kaedim3d.com/enterprise-features/custom-integrations/apis/web-api)
- [Pricing](https://www.kaedim3d.com/plans)
- [Sign up](https://docs.kaedim3d.com/welcome/get-started/sign-up)
- [Compliance](https://www.kaedim3d.com/privacy)
- [Privacy policy](https://www.kaedim3d.com/privacy)
- [GitHub](https://github.com/Kaedim)
- [Status](https://github.com/Kaedim/kaedim_status)

## API Evangelist rating

**Kin Score 48.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 22.0 |
| Contract governance | 18.2 |
| Operational transparency | 42.1 |
| Developer ergonomics | 66.1 |
| Access clarity | 73.7 |

**Agent readiness 23.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 23.6** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kaedim/](https://apis.io/providers/kaedim/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kaedim: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kaedim/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
