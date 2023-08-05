# OpenSavvy Notes Specification

> TL;DR: We are building multiple versions of the same app in multiple technical stacks to showcase the strengths of each.

Ecosystems tend to be silos of knowledge, in which developers take for granted some features and completely ignore others.
Our goal is to let developers explore how the same problems are solved in other ecosystems, to make learning easier.

To ensure easy navigation between implementations, we enforce a single REST HTTP API that all backends and frontends must conform to.
However, implementations are allowed to add new features, as long as they are still compatible with implementations which only conform to the common specification.

The repository you're currently reading is home to this common specification, as well as utilities to automatically test a specific implementation.
This specification is purposefully written in English and not in a structured format (e.g. OpenAPI) because documentation is part of the exercise: we encourage each implementation to generate its own documentation in whatever format it considers idiomatic.

## Specification

[//]: # (Will be replaced by links to subpages in the future)
