# Script deployment

## Context

The execution engine depends on scripts at runtime.
Similar technologies use various deployment mechanisms.
Deploying from the local file system simplifies deployment but lacks flexibility.
Deploying via an API decouples deployment from the runtime, but adds overhead.

## Decision

Developers will deploy scripts using the engine’s public API.

## Status

Proposed

## Consequences

* Developers will have to start the server before deploying scripts.
