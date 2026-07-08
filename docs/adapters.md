# Adapters

Adapters keep Samvad runtime-agnostic.

## Runtime Adapters

Runtime adapters connect `@samvad/server` to platforms such as Node.js, Bun, Cloudflare, and Vercel.

## Infrastructure Adapters

Infrastructure adapters implement ports defined by `@samvad/core`, such as storage, pubsub, blob, queue, and webhook delivery ports.

No package should import an adapter unless it is an app or example.
