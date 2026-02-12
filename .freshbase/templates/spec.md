---
type: spec
title: "{{TITLE}}"
context: "{{CONTEXT}}"
status: draft
version: "0.1"
---

<!--
================================================================================
GUIDE: Technical Specification (Spec)
================================================================================

WHEN TO USE
Use this type to document technical requirements for a feature.
Create a spec when:
- You have a validated feature (problem + hypothesis confirmed)
- You need to detail the "what" before the "how"
- You want to align expectations between product and engineering

REQUIRED FIELDS
- title: Descriptive name (e.g., "OAuth 2.0 Authentication")
- context: Related bounded context (e.g., "identity")
- status: draft | in_review | approved | implemented
- version: Semantic versioning (0.1, 1.0, etc.)

RELATIONSHIPS
- Born from: problem.md or hypothesis.md
- Generates: plan.md (implementation) and scenarios.md (BDD tests)
- References: context.md (bounded context) and adr.md (technical decisions)

TIPS
- Focus on the "what", not the "how" (that goes in plan.md)
- Include measurable acceptance criteria
- Link to related documents with [[wiki-style]]
- Reference problems from discovery/problems/

Delete this comment block when using the template.
================================================================================
-->

# {{TITLE}}

**Context:** [[{{CONTEXT}}]]
**Problem:** [[discovery/problems/PRB-XXX]]

## Summary

_One paragraph describing what this feature does and why it matters._

## User Stories

### Primary User Story

**As a** [user role]
**I want to** [action/goal]
**So that** [business value/outcome]

### Additional Stories

- As a... I want to... So that...

## Functional Requirements

### Must Have (P0)

1. [ ] Requirement 1
2. [ ] Requirement 2

### Should Have (P1)

1. [ ] Requirement 3

### Nice to Have (P2)

1. [ ] Requirement 4

## Non-Functional Requirements

- **Performance:** ...
- **Security:** ...
- **Accessibility:** ...

## Acceptance Criteria

```gherkin
Scenario: [Scenario name]
  Given [initial state]
  When [action]
  Then [expected outcome]
```

## Out of Scope

- _What this spec explicitly does NOT cover_

## Open Questions

- [ ] Question 1?
- [ ] Question 2?

## Related

- ADR: [[decisions/ADR-XXX]]
- Design: [link to Figma/mockups]
