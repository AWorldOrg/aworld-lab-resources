# AWorld Lab Resources

Public mirror of AWorld API schemas and TypeScript SDKs.

> **Read-only mirror.** This repository is automatically synced from an internal Bitbucket pipeline on every release. Do not open pull requests — see [CONTRIBUTING.md](./CONTRIBUTING.md).

---

## Contents

| Path | Description |
|---|---|
| [`schemas/dashboard.openapi.json`](./schemas/dashboard.openapi.json) | OpenAPI schema for the Admin API (Dashboard) |
| [`schemas/app.openapi.json`](./schemas/app.openapi.json) | OpenAPI schema for the Consumer API (App) |
| [`sdks/dashboard/`](./sdks/dashboard/) | TypeScript SDK for the Admin API — coming soon |
| [`sdks/app/`](./sdks/app/) | TypeScript SDK for the Consumer API — coming soon |

---

## Using the OpenAPI schemas

The JSON files under `schemas/` are valid OpenAPI documents. Use them with any OpenAPI-compatible tooling.

**Generate a typed client with [openapi-typescript](https://github.com/openapi-ts/openapi-typescript):**

```bash
# Dashboard (Admin API)
bunx openapi-typescript https://raw.githubusercontent.com/AWorldOrg/aworld-lab-resources/main/schemas/dashboard.openapi.json -o dashboard-schema.d.ts

# App (Consumer API)
bunx openapi-typescript https://raw.githubusercontent.com/AWorldOrg/aworld-lab-resources/main/schemas/app.openapi.json -o app-schema.d.ts
```

**Interactive API documentation (always up to date):**

https://api.aworld.org/

**Preview locally with Redoc:**

```bash
bunx @redocly/cli build-docs schemas/dashboard.openapi.json
bunx @redocly/cli build-docs schemas/app.openapi.json
```

**Raw schema URLs:**

Dashboard (Admin API):
```
https://raw.githubusercontent.com/AWorldOrg/aworld-lab-resources/main/schemas/dashboard.openapi.json
```

App (Consumer API):
```
https://raw.githubusercontent.com/AWorldOrg/aworld-lab-resources/main/schemas/app.openapi.json
```

---

## SDKs

Auto-generated TypeScript SDKs are coming soon.

- [Dashboard SDK](./sdks/dashboard/README.md) — Admin API client
- [App SDK](./sdks/app/README.md) — Consumer API client

---

## Reporting issues

Found a bug in the schema or SDK? Please [open an issue](../../issues) — do not open a pull request.
