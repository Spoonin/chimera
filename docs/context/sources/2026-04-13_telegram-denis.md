# telegram:@denis

> Ingested: 2026-04-13 · Source: telegram:@denis

## Extracted Facts

- **correction** (high): Actually deployment target is GCP, not AWS — the contract was signed last week [infrastructure, deployment]
- **question** (medium): What is the expected data volume for the first year? [database, infrastructure]
- **question** (medium): Should we use a monorepo or separate repos for each service? [architecture, ci-cd]
- **fact** (high): The staging environment is on AWS eu-west-1 [infrastructure, deployment]
- **fact** (high): The team consists of 4 backend engineers and 2 frontend engineers [team]
- **decision** (high): TypeScript for all backend services [language, architecture]
- **decision** (high): REST API for external clients, gRPC for inter-service communication [api, architecture]
- **decision** (high): Authentication will use OAuth 2.0 with PKCE flow [auth, security]
- **decision** (high): Kubernetes chosen for container orchestration in production [infrastructure, deployment]
- **decision** (high): PostgreSQL 16 selected as the primary database [database, architecture]

## Original

```
We decided to go with PostgreSQL 16 for the main DB
```
