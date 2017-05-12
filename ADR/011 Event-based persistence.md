# Event-based persistence

## Context

The engine must be able to persist script execution, so it can resume interrupted executions.
Script actions correspond to commands in a CQRS architecture.
We can model the result of executing script actions as events, as in an event sourcing architecture.

## Decision

The engine only persists events, via an event store interface, rather than its entire state.

## Status

Proposed

## Consequences

* For a simpler consistent model, the engine will persist script deployments as events.
* Querying execution states will require first reading events into a separate (generally in-memory) query model.
* Complexity still comes from dealing with snapshots, caching and clustering, replication and failover.
