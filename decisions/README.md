# Decisions

Architecture Decision Records (ADRs) for this project.

## Structure

Each decision is a markdown file following the `adr.md` template:

- `ADR-001-title.md` - First decision
- `ADR-002-title.md` - Second decision

## Template

Use the `.freshbase/templates/adr.md` template for new decisions:

```bash
cp .freshbase/templates/adr.md decisions/ADR-XXX-title.md
```

## Guidelines

- Number ADRs sequentially (ADR-001, ADR-002, etc.)
- Include status: Proposed, Accepted, Deprecated, Superseded
- Always document at least 2 alternatives considered
- Link to related specs and contexts
