# Context Map

> Domain-Driven Design bounded contexts for this project.

## Overview

This document serves as the central registry of all bounded contexts in the project.
Each context represents a distinct subdomain with clear boundaries and responsibilities.

## Contexts

| Context | Description | Status |
|---------|-------------|--------|
| _Example_ | _Add your first bounded context_ | _Discovery_ |

## Relationships

```
[Context A] <-- [upstream/downstream] --> [Context B]
```

## Guidelines

### Creating a New Context

1. Create a folder under `contexts/{context-name}/`
2. Add a `context.md` file using the template
3. Define the domain language (ubiquitous language)
4. List key features and link to specs

### Context Boundaries

- Each context should have a **single responsibility**
- Minimize dependencies between contexts
- Use **Anti-Corruption Layers** when integrating with external systems

## Related

- [[discovery/problems/]] - Problems driving context creation
- [[decisions/]] - ADRs about context boundaries
