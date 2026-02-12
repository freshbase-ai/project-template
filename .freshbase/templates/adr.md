---
type: adr
title: "{{TITLE}}"
status: proposed
deciders: "{{DECIDERS}}"
date: "{{DATE}}"
---

<!--
================================================================================
GUIDE: Architecture Decision Record (ADR)
================================================================================

WHEN TO USE
Use this type to record important architectural decisions.
Create an ADR when:
- Making a significant technical decision
- Choosing between alternatives with trade-offs
- Needing to document the "why" behind a choice

REQUIRED FIELDS
- title: Descriptive name (e.g., "Use Stripe for payments")
- status: proposed | accepted | deprecated | superseded
- deciders: List of people who participated in the decision
- date: Date of the decision

RELATIONSHIPS
- Born from: Discussions in meetings or needs from specs
- References: affected specs and contexts
- Can be superseded by: another more recent ADR

TIPS
- Always document at least 2 alternatives considered
- Include pros/cons for each alternative
- Clearly explain why an alternative was rejected
- Use active voice: "We will use X because Y"

Delete this comment block when using the template.
================================================================================
-->

# {{TITLE}}

## Context

_Describe the context and problem that motivates this decision._

## Decision

_Describe the decision taken. Use active voice: "We will use X because Y"_

## Consequences

### Positive

- _Benefit 1_
- _Benefit 2_

### Negative

- _Trade-off 1_
- _Risk to mitigate_

### Neutral

- _Changes we need to make_

## Alternatives Considered

### Option 1: _Name_

**Pros:** ...
**Cons:** ...
**Why rejected:** ...

### Option 2: _Name_

**Pros:** ...
**Cons:** ...
**Why rejected:** ...

## Related

- Supersedes: ADR-XXX (if applicable)
- Related specs: [[specs/{{FEATURE}}]]
- Related contexts: [[contexts/{{CONTEXT}}]]
