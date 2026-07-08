# Architecture

Samvad is runtime-agnostic chat infrastructure.

The architecture is layered:

- `@samvad/protocol` defines the public wire contract.
- `@samvad/core` owns the Effect-powered domain and service boundaries.
- `@samvad/server` composes runtime-neutral HTTP and WebSocket handling.
- Runtime adapters connect the server layer to deployment platforms.
- Infrastructure adapters implement core ports for storage, pubsub, blobs, queues, and webhooks.

Product-specific logic belongs in the user's backend. Samvad only understands participants, conversations, messages, membership, presence, read state, events, and webhooks.
