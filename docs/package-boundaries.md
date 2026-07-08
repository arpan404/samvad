# Package Boundaries

## `@samvad/protocol`

Allowed imports: none from Samvad packages.

Disallowed imports: runtime APIs, server code, databases, WebSocket libraries, Redis, Postgres, Node APIs, Bun APIs, and Cloudflare APIs.

## `@samvad/core`

Allowed imports: Effect and `@samvad/protocol`.

Disallowed imports: Node, Bun, Cloudflare, Vercel, Redis, Postgres, WebSocket libraries, and HTTP framework code.

## `@samvad/server`

Allowed imports: `@samvad/core` and `@samvad/protocol`.

Disallowed imports: Node, Bun, Cloudflare, Vercel, Redis, and Postgres runtime-specific APIs.

## `@samvad/client`

Allowed imports: `@samvad/protocol`.

Disallowed imports: React and server/runtime adapter code.

## Runtime Adapters

Allowed imports: `@samvad/server`, `@samvad/core`, and `@samvad/protocol` as needed.

Runtime adapters must not be imported by protocol, core, server, or client packages.

## Infrastructure Adapters

Allowed imports: `@samvad/core` and `@samvad/protocol` as needed.

Infrastructure adapters must not be imported by protocol, core, server, or client packages.

## Apps and Examples

Apps and examples may import adapters to demonstrate real deployments.
