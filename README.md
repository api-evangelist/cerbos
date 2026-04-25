# Cerbos (cerbos)
Cerbos is an open-core, language-agnostic, scalable authorization platform that decouples access control from application code by externalizing fine-grained, context-aware permission decisions into policy-as-code. Authorization is expressed in YAML policies supporting RBAC, ABAC, PBAC, and ReBAC, evaluated by a stateless Policy Decision Point (PDP) that delivers sub-millisecond decisions at scale. The platform consists of the open-source Cerbos PDP (Apache 2.0), Cerbos Hub control plane (PAP), Cerbos Synapse enrichment layer, and PEP SDKs for Go, Java, JavaScript / TypeScript, .NET, PHP, Python, Ruby, and Rust. The PDP exposes both REST (port 3592) and gRPC (port 3593) interfaces, an Admin API, and standards-compliant OpenID AuthZEN endpoints, with query-plan adapters for Prisma and SQLAlchemy.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Authorization, Access Control, Policy as Code, RBAC, ABAC, PBAC, ReBAC, AuthZEN, PDP, Permissions, Open Source, Zero Trust

## Timestamps

- **Created:** 2026-03-25
- **Modified:** 2026-04-23

## APIs

### Cerbos PDP REST API
The Cerbos PDP REST API is the HTTP/JSON interface for sending authorization requests to a running Cerbos Policy Decision Point. It exposes CheckResources, PlanResources, and ServerInfo endpoints, with an OpenAPI / Swagger specification served by every PDP.

**Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)

**Base URL:** `http://localhost:3592`

#### Tags
- REST, PDP, CheckResources, PlanResources

#### Properties
- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index)
- [OpenAPI](https://docs.cerbos.dev/cerbos/latest/api/swagger.json)
- [Reference](https://docs.cerbos.dev/cerbos/latest/api/index#api-resources)

### Cerbos PDP gRPC API
The Cerbos PDP gRPC API exposes the cerbos.svc.v1.CerbosService and related management services on port 3593, with server reflection enabled.

**Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)

**Base URL:** `localhost:3593`

#### Tags
- gRPC, PDP, Protocol Buffers

#### Properties
- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index)
- [Protocol](https://github.com/cerbos/cerbos/tree/main/api/genpb)

### Cerbos AuthZEN API
Cerbos implements the OpenID AuthZEN authorization API specification, exposing standards-compliant single-evaluation, batch-evaluations, and well-known metadata endpoints.

**Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/index](https://docs.cerbos.dev/cerbos/latest/api/index)

#### Tags
- AuthZEN, OpenID, Standards

#### Properties
- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/index#authzen)
- [Specification](https://openid.net/specs/authorization-api-1_0.html)

### Cerbos PDP Admin API
Provides management capabilities such as policy add/get/list, schema management, and audit log access on the running PDP. Gated by HTTP Basic Auth.

**Human URL:** [https://docs.cerbos.dev/cerbos/latest/api/admin_api](https://docs.cerbos.dev/cerbos/latest/api/admin_api)

#### Tags
- Admin, Policy Management, Audit Log

#### Properties
- [Documentation](https://docs.cerbos.dev/cerbos/latest/api/admin_api)

### Cerbos Hub API
Cerbos Hub is the cloud-hosted Policy Administration Point (PAP) that manages policy authoring, versioning, validation, and distribution to Cerbos PDPs.

**Human URL:** [https://docs.cerbos.dev/cerbos-hub/](https://docs.cerbos.dev/cerbos-hub/)

#### Tags
- Hub, Cloud, Policy Administration, Policy Distribution

#### Properties
- [Documentation](https://docs.cerbos.dev/cerbos-hub/)
- [Console](https://hub.cerbos.cloud/)

### Cerbos Synapse
Synapse is the enrichment and orchestration component that fetches identity, resource, and relationship attributes from external systems and translates infrastructure protocols into Cerbos authorization checks for ReBAC and ABAC.

**Human URL:** [https://www.cerbos.dev/products/synapse](https://www.cerbos.dev/products/synapse)

#### Tags
- Synapse, Enrichment, ReBAC

#### Properties
- [Documentation](https://www.cerbos.dev/products/synapse)

## Common Properties

- [Website](https://www.cerbos.dev)
- [Documentation](https://docs.cerbos.dev)
- [GettingStarted](https://docs.cerbos.dev/cerbos/latest/quickstart)
- [API](https://docs.cerbos.dev/cerbos/latest/api/index)
- [OpenAPI](https://docs.cerbos.dev/cerbos/latest/api/swagger.json)
- [Hub](https://hub.cerbos.cloud/)
- [GitHub](https://github.com/cerbos/cerbos)
- [SourceCode](https://github.com/cerbos/cerbos)
- [IssueTracker](https://github.com/cerbos/cerbos/issues)
- [Releases](https://github.com/cerbos/cerbos/releases)
- [Blog](https://www.cerbos.dev/blog)
- [Pricing](https://www.cerbos.dev/pricing)
- [Slack](https://join.slack.com/t/cerbos/shared_invite/zt-1a99bp8d6-fJiaY7lpDRRUe4UB1u35Yw)
- [X](https://x.com/CerbosDev)
- [LinkedIn](https://www.linkedin.com/company/cerbos)
- [YouTube](https://www.youtube.com/@cerbos)
- [License](https://github.com/cerbos/cerbos/blob/main/LICENSE)
- [Playground](https://play.cerbos.dev)
- [DockerHub](https://hub.docker.com/r/cerbos/cerbos)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
