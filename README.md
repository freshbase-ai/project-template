# {{PROJECT_NAME}}

This is a discovery and planning workspace managed by Freshbase v2.0.

## Getting Started

1. Explore the templates in `.freshbase/templates/`
2. Each template is self-documenting - read the guide at the beginning
3. Create documents wherever makes sense for your project
4. The system identifies documents by the `type:` field in the frontmatter

## Documentation

- **Templates:** `.freshbase/templates/`
- **Configuration:** `.freshbase/config.yaml`
- **Principles:** `.freshbase/constitution.md`

## Document Types

| Type | When to Use |
|------|-------------|
| `spec` | Specify technical requirements |
| `adr` | Record architectural decisions |
| `meeting` | Document meetings |
| `context` | Define bounded contexts |
| `problem` | Capture business problems |
| `hypothesis` | Validate hypotheses |
| `flow` | Map cross-context flows |
| `plan` | Plan implementation |
| `scenarios` | Write BDD scenarios |

## Core Principle

> The type of a document is defined by its metadata (frontmatter `type:`),
> not by the folder where it is saved.

Organize your files however you prefer. The system will find them by type.

---
*Workspace managed by Freshbase v2.0*
