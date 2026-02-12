---
type: context
title: "{{CONTEXT_NAME}}"
responsibility: "{{RESPONSIBILITY}}"
---

<!--
================================================================================
GUIDE: Bounded Context (Context)
================================================================================

WHEN TO USE
Use this type to define bounded contexts (DDD).
Create a context when:
- Identifying a distinct subdomain in the system
- Needing to define clear boundaries of responsibility
- Wanting to establish the ubiquitous language of the domain

REQUIRED FIELDS
- title: Bounded context name (e.g., "Identity & Authentication")
- responsibility: Summary of the main responsibility

RELATIONSHIPS
- Contains: specs (context features)
- References: ADRs about context decisions
- Relates to: other contexts (upstream/downstream)

TIPS
- Clearly define what the context DOES and DOES NOT do
- Create a glossary with domain language
- Minimize dependencies between contexts
- Use Anti-Corruption Layers for external integration

Delete this comment block when using the template.
================================================================================
-->

# {{CONTEXT_NAME}}

> **Definition:** What this bounded context does and DOES NOT do.

## Responsibility

**This context IS responsible for:**
- ...

**This context IS NOT responsible for:**
- ...

## Domain Language

| Term | Definition |
|------|------------|
| _Example Term_ | _Clear definition in business language_ |

## Key Features

- [[specs/{{FEATURE}}/spec.md]]

## Dependencies

### Upstream (this context depends on)

- None

### Downstream (depends on this context)

- None

## Integration Points

| System | Direction | Protocol | Notes |
|--------|-----------|----------|-------|
| _External API_ | _Inbound_ | _REST_ | _Description_ |

## Related

- ADRs: [[decisions/ADR-XXX]]
- Flows: [[flows/{{FLOW}}]]
