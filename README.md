# Samvad

Self-hosted, runtime-agnostic chat infrastructure for adding realtime messaging to any app.

Samvad is protocol-first and built around Effect-powered core services with runtime and infrastructure adapters at the edges.

## Packages

- `@samvad/protocol`: public frames, events, schemas, constants, and error codes.
- `@samvad/core`: Effect-powered chat engine interfaces and domain boundaries.
- `@samvad/server`: runtime-neutral HTTP and WebSocket server composition.
- `@samvad/client`: browser/runtime-neutral client SDK.
- `@samvad/adapter-*`: runtime and infrastructure adapters.

## Commands

```sh
bun install
bun run build
bun run test
bun run lint
bun run typecheck
```

## Status

This repository currently contains project structure, package boundaries, configuration, and documentation stubs only. Chat business logic has not been implemented yet.
