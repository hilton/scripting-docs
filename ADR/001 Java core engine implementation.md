# ADR-1 Java core engine implementation

## Context

We can choose between several popular server development languages that we have experience with and which would be suitable for building server software.
The newest languages offer other programming styles, such as functional programming, and other potential benefits compared to older languages.
Meanwhile, older languages such as Java offer a much richer enterprise integration ecosystem, and far wider adoption in enterprise environments.
Also, given an existing team, the best language choice is usually the one the team has the most experience with.

## Decision

We will implement the core engine in Java.

## Status

Accepted

## Consequences

We will select a Java HTTP API to use.
