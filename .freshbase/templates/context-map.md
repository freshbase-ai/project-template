---
title: "{{TITLE}}"
---

<!--
================================================================================
GUIDE: Context Map
================================================================================

WHEN TO USE
Use this template to map features that cross multiple bounded contexts.
Create a context-map when:
- A feature involves 2+ bounded contexts
- You need to document integrations between contexts
- You want to visualize data flow between domains

SUGGESTED FIELDS
- title: Descriptive name (e.g., "Cross-Context Feature: User Onboarding")

RELATIONSHIPS
- References: involved contexts
- Complements: flow.md (step sequence)
- Documents: integration decisions (ADRs)

TIPS
- Identify the "owner" context of the feature
- Document integration contracts (APIs, events)
- Specify consistency model (strong vs eventual)
- List integration risks and mitigations

Delete this comment block when using the template.
================================================================================
-->

# Context Map: {{TITLE}}

## Overview

{Description of the feature that crosses multiple contexts}

## Affected Contexts

### Primary Context

- **Context:** [[contexts/{{PRIMARY_CONTEXT}}]]
- **Role:** Owner / Coordinator
- **Responsibilities:** {what this context manages}

### Secondary Contexts

#### {{CONTEXT_NAME_1}}

- **Context:** [[contexts/{{CONTEXT_1}}]]
- **Role:** Supplier / Consumer
- **Integration:** {integration type - API, Events, Shared Kernel}
- **Contract:** {contract description}

#### {{CONTEXT_NAME_2}}

- **Context:** [[contexts/{{CONTEXT_2}}]]
- **Role:** Supplier / Consumer
- **Integration:** {integration type}
- **Contract:** {contract description}

## Integration Patterns

### Data Flow

```
[Context A] --event--> [Context B] --API--> [Context C]
```

### Shared Types

- `{TypeName}`: used by {Context A, Context B}
- `{TypeName}`: used by {Context B, Context C}

## Coordination

### Orchestration vs Choreography

{Describe whether there is a central orchestrator or event-based choreography}

### Consistency Model

- **Strong Consistency:** {which operations}
- **Eventual Consistency:** {which operations}

## Risks & Considerations

- {Risk 1}: {mitigation}
- {Risk 2}: {mitigation}

## Related

- **Flow:** [[flows/{{FLOW}}]]
- **Specs:** [[specs/{{SPEC}}]]
