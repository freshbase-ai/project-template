---
title: "{{TITLE}}"
---

<!--
================================================================================
GUIA: Context Map (Mapa de Contextos)
================================================================================

QUANDO USAR
Use este template para mapear features que cruzam multiplos bounded contexts.
Crie um context-map quando:
- Uma feature envolve 2+ bounded contexts
- Precisa documentar integracoes entre contextos
- Quer visualizar o fluxo de dados entre dominios

CAMPOS SUGERIDOS
- title: Nome descritivo (ex: "Feature Cross-Context: User Onboarding")

RELACIONAMENTOS
- Referencia: contexts envolvidos
- Complementa: flow.md (sequencia de passos)
- Documenta: decisoes de integracao (ADRs)

DICAS
- Identifique o contexto "owner" da feature
- Documente contratos de integracao (APIs, eventos)
- Especifique modelo de consistencia (strong vs eventual)
- Liste riscos de integracao e mitigacoes

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# Context Map: {{TITLE}}

## Overview

{Descricao da feature que cruza multiplos contextos}

## Affected Contexts

### Primary Context

- **Context:** [[contexts/{{PRIMARY_CONTEXT}}]]
- **Role:** Owner / Coordinator
- **Responsibilities:** {o que este contexto gerencia}

### Secondary Contexts

#### {{CONTEXT_NAME_1}}

- **Context:** [[contexts/{{CONTEXT_1}}]]
- **Role:** Supplier / Consumer
- **Integration:** {tipo de integracao - API, Events, Shared Kernel}
- **Contract:** {descricao do contrato}

#### {{CONTEXT_NAME_2}}

- **Context:** [[contexts/{{CONTEXT_2}}]]
- **Role:** Supplier / Consumer
- **Integration:** {tipo de integracao}
- **Contract:** {descricao do contrato}

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

{Descrever se ha um orquestrador central ou se e coreografia baseada em eventos}

### Consistency Model

- **Strong Consistency:** {quais operacoes}
- **Eventual Consistency:** {quais operacoes}

## Risks & Considerations

- {Risk 1}: {mitigation}
- {Risk 2}: {mitigation}

## Related

- **Flow:** [[flows/{{FLOW}}]]
- **Specs:** [[specs/{{SPEC}}]]
