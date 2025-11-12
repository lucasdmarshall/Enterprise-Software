# Backend

APIs and services, plus shared backend packages.

Suggested layout:
- `services/api/` – Public API gateway (REST/GraphQL).
- `services/gateway/` – BFF or edge gateway.
- `packages/core/` – Domain orchestration and application services.
- `packages/shared/` – Shared backend utilities/types.

Implement with your preferred stack (e.g., Node/Express/Nest, .NET, Python/FastAPI).