---
type: plan
title: "{{TITLE}}"
spec: "{{SPEC_REFERENCE}}"
status: planning
owner: "{{OWNER}}"
effort: M
---

<!--
================================================================================
GUIDE: Implementation Plan (Plan)
================================================================================

WHEN TO USE
Use this type to plan the implementation of a spec.
Create a plan when:
- A spec has been approved and is ready for implementation
- You need to break work into smaller tasks
- You want to track progress and dependencies

REQUIRED FIELDS
- title: Descriptive name (e.g., "Implementation: One-click Checkout")
- spec: Reference to the spec being implemented
- status: planning | in_progress | blocked | completed

OPTIONAL FIELDS
- owner: Responsible for implementation
- effort: S | M | L | XL (effort estimate)

RELATIONSHIPS
- Born from: approved spec
- Breaks into: tasks/implementation phases
- References: ADRs for technical decisions

TIPS
- Divide into logical phases (Foundation, Core, Integration)
- Include prerequisites and dependencies
- Maintain a progress log
- Define clear "done" criteria

Delete this comment block when using the template.
================================================================================
-->

# {{TITLE}}

**Spec:** [[specs/{{SPEC}}]]
**Bounded Context:** [[contexts/{{CONTEXT}}]]

## Prerequisites

- [ ] Dependency 1 completed
- [ ] Dependency 2 available

## Implementation Steps

### Phase 1: Foundation

- [ ] **Task 1.1:** Description
  - Details or sub-tasks
- [ ] **Task 1.2:** Description

### Phase 2: Core Implementation

- [ ] **Task 2.1:** Description
- [ ] **Task 2.2:** Description

### Phase 3: Integration & Testing

- [ ] **Task 3.1:** Write unit tests
- [ ] **Task 3.2:** Integration testing
- [ ] **Task 3.3:** Documentation updates

## Technical Notes

_Any architectural decisions, patterns, or considerations._

## Risks & Mitigations

| Risk | Impact | Mitigation |
|------|--------|------------|
| _Risk description_ | _High/Med/Low_ | _How to address_ |

## Definition of Done

- [ ] All acceptance criteria from spec met
- [ ] Tests passing (unit + integration)
- [ ] Documentation updated
- [ ] Code reviewed and approved
- [ ] Deployed to staging

## Progress Log

| Date | Update |
|------|--------|
| {{DATE}} | Plan created |
