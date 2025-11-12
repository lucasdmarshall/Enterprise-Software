# Architecture

## High-Level Layout

- Frontend apps live in `frontend/apps/*` and consume backend APIs.
- Backend services live in `backend/services/*` and expose transport (HTTP/GraphQL/gRPC).
- Domain logic is centralized in `modules/*` and shared across services.
- Integrations (payment gateways, tax providers, analytics) live in `plugins/*`.
- Database migrations/seeders/schemas live in `database/*`.
- Hardware drivers and device adapters live in `hardware/*`.

## Boundaries & Principles

- Separation of concerns: UI vs transport vs domain.
- Contract-first interfaces between `backend` and `modules`.
- Plugins follow adapter pattern to keep core domain stable.
- Hardware integrations are abstracted via drivers and device-specific adapters.