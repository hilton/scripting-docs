# ADR-3 Core model naming

## Context

In process engine implementations, we refer to processes or workflows, made up of activities, and executed by cases.
However, processes and workflows have failed to become popular among developers.
We can initially focus on microservice orchestration by using naming based on script and service execution.

## Decision

Use programmer-centric naming based on microservices and script execution, instead of process engine naming.

## Status

Proposed

## Consequences

* Developers will understand the model more quickly but will not assume standard process engine functionality like asynchronous parallel execution.
* We may produce documentation that explains the engine for people more familiar with workflow or BPM.
* We can always present the engine differently for use cases other than microservice orchestration.
