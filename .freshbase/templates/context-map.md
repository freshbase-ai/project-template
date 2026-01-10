# Context Map: {FEATURE-TITLE}

## Overview
{Descrição da feature que cruza múltiplos contextos}

## Affected Contexts

### Primary Context
- **Context:** [[contexts/{primary-context}]]
- **Role:** Owner / Coordinator
- **Responsibilities:** {o que este contexto gerencia}

### Secondary Contexts

#### {Context Name 1}
- **Context:** [[contexts/{context-1}]]
- **Role:** Supplier / Consumer
- **Integration:** {tipo de integração - API, Events, Shared Kernel}
- **Contract:** {descrição do contrato}

#### {Context Name 2}
- **Context:** [[contexts/{context-2}]]
- **Role:** Supplier / Consumer
- **Integration:** {tipo de integração}
- **Contract:** {descrição do contrato}

## Integration Patterns

### Data Flow
```
[Context A] --event--> [Context B] --API--> [Context C]
```

### Shared Types
- `{TypeName}`: usado por {Context A, Context B}
- `{TypeName}`: usado por {Context B, Context C}

## Coordination

### Orchestration vs Choreography
{Descrever se há um orquestrador central ou se é coreografia baseada em eventos}

### Consistency Model
- **Strong Consistency:** {quais operações}
- **Eventual Consistency:** {quais operações}

## Risks & Considerations
- {Risk 1}: {mitigation}
- {Risk 2}: {mitigation}

## Related
- **Spec:** [[cross-cutting/{feature-id}/spec.md]]
- **Scenarios:** [[cross-cutting/{feature-id}/scenarios.md]]
