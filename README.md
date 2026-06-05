# Cerbos (cerbos)

Cerbos is an open-core, language-agnostic, scalable authorization platform that decouples access control from application code by externalizing fine-grained, context-aware permission decisions into policy-as-code. Authorization is expressed in YAML policies supporting RBAC, ABAC, PBAC, and ReBAC, evaluated by a stateless Policy Decision Point (PDP) that delivers sub-millisecond decisions at scale. The platform consists of the open-source Cerbos PDP (Apache 2.0), Cerbos Hub control plane (PAP), Cerbos Synapse enrichment layer, and PEP SDKs for Go, Java, JavaScript / TypeScript, .NET, PHP, Python, Ruby, and Rust. The PDP exposes both REST (port 3592) and gRPC (port 3593) interfaces, an Admin API, and standards- compliant OpenID AuthZEN endpoints, with query-plan adapters for Prisma and SQLAlchemy.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- ABAC
- Access Control
- Authorization
- AuthZEN
- Open Source
- PBAC
- PDP
- Permissions
- Policy as Code
- RBAC
- ReBAC
- Zero Trust

## Timestamps

- **Created:** 2026-03-25
- **Modified:** 2026-05-19

## APIs

### Cerbos PDP REST API

The Cerbos PDP REST API is the HTTP/JSON interface for sending authorization requests to a running Cerbos Policy Decision Point. It exposes CheckResources for evaluating principal-against-resource decisions, PlanResources for translating policies into resource-filter query plans, and ServerInfo for runtime metadata. An OpenAPI / Swagger specification is served by every PDP instance.

- **Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)
- **Base URL:** `http://localhost:3592`

#### Tags

- CheckResources
- PDP
- PlanResources
- REST

#### Properties

- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index)
- [OpenAPI](https://docs.cerbos.dev/cerbos/latest/api/swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Reference](https://docs.cerbos.dev/cerbos/latest/api/index#api-resources)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cerbos PDP gRPC API

The Cerbos PDP gRPC API exposes the cerbos.svc.v1.CerbosService and related management services on port 3593, with server reflection enabled. The gRPC interface is the highest-performance way to embed Cerbos as a sidecar or in-process service for service-to-service authorization.

- **Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)
- **Base URL:** `localhost:3593`

#### Tags

- gRPC
- PDP
- Protocol Buffers

#### Properties

- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index)
- [Protocol](https://github.com/cerbos/cerbos/tree/main/api/genpb)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cerbos AuthZEN API

Cerbos implements the OpenID AuthZEN authorization API specification, exposing standards-compliant single-evaluation, batch-evaluations, and well-known metadata endpoints so that any AuthZEN-conformant client or Policy Enforcement Point can integrate with Cerbos as the decision engine.

- **Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)

#### Tags

- AuthZEN
- OpenID
- Standards

#### Properties

- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index#authzen)
- [Specification](https://openid.net/specs/authorization-api-1_0.html)
- [Discovery](https://docs.cerbos.dev/cerbos/latest/api/index#authzen)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cerbos PDP Admin API

The Cerbos Admin API provides management capabilities such as policy add/get/list, schema management, and audit log access on the running PDP. It is intended for administrative use and is gated by HTTP Basic Auth.

- **Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/admin_api](https://docs.cerbos.dev/cerbos/latest/api/admin_api)

#### Tags

- Admin
- Audit Log
- Policy Management

#### Properties

- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/admin_api)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cerbos Hub API

Cerbos Hub is the cloud-hosted Policy Administration Point (PAP) that manages policy authoring, versioning, validation, and distribution to Cerbos PDPs across environments. It also provides decision logs, collaborative policy editing, and embedded PDP delivery.

- **Human URL:** [https://docs.cerbos.dev/cerbos-hub/](https://docs.cerbos.dev/cerbos-hub/)

#### Tags

- Cloud
- Hub
- Policy Administration
- Policy Distribution

#### Properties

- [Documentation](https://docs.cerbos.dev/cerbos-hub/)
- [Console](https://hub.cerbos.cloud/)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cerbos Synapse

Cerbos Synapse is the enrichment and orchestration component that fetches identity, resource, and relationship attributes from external systems and translates infrastructure protocols (HTTP, gRPC, GraphQL) into Cerbos authorization checks for ReBAC and ABAC scenarios.

- **Human URL:** [https://www.cerbos.dev/products/synapse](https://www.cerbos.dev/products/synapse)

#### Tags

- Enrichment
- ReBAC
- Synapse

#### Properties

- [Documentation](https://www.cerbos.dev/products/synapse)
- [Postman Collection](collections/cerbos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cerbos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.cerbos.dev)
- [Documentation](https://docs.cerbos.dev)
- [Getting Started](https://docs.cerbos.dev/cerbos/latest/quickstart)
- [A P I](https://docs.cerbos.dev/cerbos/latest/api/index)
- [OpenAPI](https://docs.cerbos.dev/cerbos/latest/api/swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Hub](https://hub.cerbos.cloud/)
- [Git Hub](https://github.com/cerbos/cerbos)
- [GitHub Organization](https://github.com/cerbos)
- [Source Code](https://github.com/cerbos/cerbos)
- [Issue Tracker](https://github.com/cerbos/cerbos/issues)
- [Releases](https://github.com/cerbos/cerbos/releases)
- [Blog](https://www.cerbos.dev/blog)
- [Pricing](https://www.cerbos.dev/pricing)
- [Case Studies](https://www.cerbos.dev/case-studies)
- [Customers](https://www.cerbos.dev/customers)
- [Slack](https://join.slack.com/t/cerbos/shared_invite/zt-1a99bp8d6-fJiaY7lpDRRUe4UB1u35Yw)
- [X (Twitter)](https://x.com/CerbosDev)
- [LinkedIn](https://www.linkedin.com/company/cerbos)
- [YouTube](https://www.youtube.com/@cerbos)
- [License](https://github.com/cerbos/cerbos/blob/main/LICENSE)
- [Security Policy](https://www.cerbos.dev/security)
- [Terms of Service](https://www.cerbos.dev/terms)
- [Privacy Policy](https://www.cerbos.dev/privacy)
- [Playground](https://play.cerbos.dev)
- [Docker Hub](https://hub.docker.com/r/cerbos/cerbos)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [S D Ks](undefined)
- [Integrations](https://www.cerbos.dev/ecosystem)
- [Agent Skill](https://github.com/cerbos/skills)
- [L L Ms Txt](https://docs.cerbos.dev/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
