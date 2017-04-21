# Language drivers

## Context

A polyglot approach will help adoption, and make the engine available to the most developers.
However, supporting multiple languages will slow down initial development.
Developing initially for only one language risks tying the implementation to that language.
We can prioritise the most popular languages.

## Decision

Write language drivers for Java and JavaScript (i.e. ECMAScript 2017) to start with.

## Status

Accepted

## Consequences

Writing driver APIs for languages both with and without static types may lead to multiple strategies for ensuring script correctness at runtime.
