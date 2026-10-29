# Cerbos

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

Cerbos is an open-core, language-agnostic, scalable authorization platform that decouples access control from application code by externalizing fine-grained, context-aware permission decisions into policy-as-code. Authorization is expressed in YAML policies supporting RBAC, ABAC, PBAC, and ReBAC, evaluated by a stateless Policy Decision Point (PDP) that delivers sub-millisecond decisions at scale. The platform consists of the open-source Cerbos PDP (Apache 2.0), Cerbos Hub control plane (PAP), Cerbos Synapse enrichment layer, and PEP SDKs for Go, Java, JavaScript / TypeScript, .NET, PHP, Python, Ruby, and Rust. The PDP exposes both REST (port 3592) and gRPC (port 3593) interfaces, an Admin API, and standards- compliant OpenID AuthZEN endpoints, with query-plan adapters for Prisma and SQLAlchemy.

**Areas:** ABAC · Access Control · Authorization · AuthZEN · Open Source · PBAC · PDP · Permissions · Policy as Code · RBAC · ReBAC · Zero Trust

## Cerbos on APIs.io

Everything profiled for Cerbos is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/cerbos/](https://apis.io/providers/cerbos/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Cerbos PDP gRPC API](https://apis.io/apis/cerbos/cerbos-pdp-grpc-api/) — The Cerbos PDP gRPC API exposes the cerbos.svc.v1.CerbosService and related management services on port 3593, with server reflection enabled. The gRPC…
- [Cerbos AuthZEN API](https://apis.io/apis/cerbos/cerbos-authzen-api/) — Cerbos implements the OpenID AuthZEN authorization API specification, exposing standards-compliant single-evaluation, batch-evaluations, and well-known…
- [Cerbos PDP Admin API](https://apis.io/apis/cerbos/cerbos-admin-api/) — The Cerbos Admin API provides management capabilities such as policy add/get/list, schema management, and audit log access on the running PDP. It is…
- [Cerbos Hub API](https://apis.io/apis/cerbos/cerbos-hub-api/) — Cerbos Hub is the cloud-hosted Policy Administration Point (PAP) that manages policy authoring, versioning, validation, and distribution to Cerbos PDPs…
- [Cerbos Synapse](https://apis.io/apis/cerbos/cerbos-synapse/) — Cerbos Synapse is the enrichment and orchestration component that fetches identity, resource, and relationship attributes from external systems and…
- [Cerbos Admin Audit API](https://apis.io/apis/cerbos/cerbos-admin-audit-api/) — Audit and decision log access (Admin API).
- [Cerbos Admin Policies API](https://apis.io/apis/cerbos/cerbos-admin-policies-api/) — Policy management (Admin API).
- [Cerbos Admin Schemas API](https://apis.io/apis/cerbos/cerbos-admin-schemas-api/) — JSON schema management (Admin API).
- [Cerbos Admin Store API](https://apis.io/apis/cerbos/cerbos-admin-store-api/) — Policy store administration (Admin API).
- [Cerbos Check API](https://apis.io/apis/cerbos/cerbos-check-api/) — Evaluate authorization decisions.
- [Cerbos Plan API](https://apis.io/apis/cerbos/cerbos-plan-api/) — Generate query plans for resource filtering.
- [Cerbos Server API](https://apis.io/apis/cerbos/cerbos-server-api/) — PDP server metadata.
- [Cerbos Auth ZEN API](https://apis.io/apis/cerbos/cerbos-auth-zen-api/) — OpenID AuthZEN standards-compliant evaluation endpoints.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/cerbos/](https://apis.io/graphqls/cerbos/cerbos-graphql/)

#### Agent skills (1)

Agent skills built on the API.

- [cerbos-policy](https://apis.io/agent-skills/cerbos/cerbos-policy/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Cerbos Agentic Access](https://apis.io/agentic-access/cerbos/cerbos-agentic-access/)

#### Collections (9)

Postman and Open Collection request collections.

- [Cerbos PDP REST API](https://apis.io/collections/cerbos/open-cerbos/)
- [Cerbos PDP REST Admin Audit API](https://apis.io/collections/cerbos/open-cerbos-admin-audit-api/)
- [Cerbos PDP REST Admin Audit Admin Policies API](https://apis.io/collections/cerbos/open-cerbos-admin-policies-api/)
- [Cerbos PDP REST Admin Audit Admin Schemas API](https://apis.io/collections/cerbos/open-cerbos-admin-schemas-api/)
- [Cerbos PDP REST Admin Audit Admin Store API](https://apis.io/collections/cerbos/open-cerbos-admin-store-api/)
- [Cerbos PDP REST Admin Audit AuthZEN API](https://apis.io/collections/cerbos/open-cerbos-authzen-api/)
- [Cerbos PDP REST Admin Audit Check API](https://apis.io/collections/cerbos/open-cerbos-check-api/)
- [Cerbos PDP REST Admin Audit Plan API](https://apis.io/collections/cerbos/open-cerbos-plan-api/)
- [Cerbos PDP REST Admin Audit Server API](https://apis.io/collections/cerbos/open-cerbos-server-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Cerbos Authentication](https://apis.io/security/cerbos/cerbos-authentication/)
- [Cerbos Domain Security](https://apis.io/security/cerbos/cerbos-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Cerbos Plans Pricing](https://apis.io/plans/cerbos/cerbos-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Cerbos Rate Limits](https://apis.io/rate-limits/cerbos/cerbos-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Cerbos Finops](https://apis.io/finops/cerbos/cerbos-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.cerbos.dev)
- [Documentation](https://docs.cerbos.dev)
- [Getting started](https://docs.cerbos.dev/cerbos/latest/quickstart)
- [Pricing](https://www.cerbos.dev/pricing)
- [Blog](https://www.cerbos.dev/blog)
- [Terms of service](https://www.cerbos.dev/terms)
- [Privacy policy](https://www.cerbos.dev/privacy)
- [GitHub](https://github.com/cerbos)

## API Evangelist rating

**Kin Score 42.7** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 42.2 |
| Contract governance | 0.0 |
| Operational transparency | 36.8 |
| Developer ergonomics | 68.3 |
| Access clarity | 18.4 |

**Agent readiness 22.8** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | unknown |
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

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/cerbos/](https://apis.io/providers/cerbos/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Cerbos: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/cerbos/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
