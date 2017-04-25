# Script deployment

## Context

The execution engine depends on scripts at runtime.
Similar technologies use various deployment mechanisms.
Deploying from the local file system simplifies deployment but lacks flexibility.
Deploying via an API decouples deployment from the runtime, but adds overhead.

## Decision

Developers will deploy scripts using the engine’s public API, typically as part of their own service start-up.

## Status

Proposed

## Consequences

* Developers will have to start the server before deploying scripts.
* Script deployment must use idempotent commands, so that services using a programmatic API can always attempt to deploy without having to know if they’ve deployed before.
