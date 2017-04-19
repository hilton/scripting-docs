# ADR-4 JSON script syntax

## Context

Scripts define service orchestration declaratively, with different structures to existing programming languages.
Meanwhile, we support developers who use various languages.
Scripts could use a new language, or an existing data-serialisation format.
A new language would add overhead, both to implement and for developers to learn.
XML-based script languages teach us that we should avoid XML for this.

## Decision

Use JSON for the canonical script syntax.

## Status

Accepted

## Consequences

* Script deployment requires custom script validation (‘compilation’).
* A good developer experience requires a language driver API for script authoring.
