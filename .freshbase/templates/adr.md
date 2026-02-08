---
type: adr
title: "{{TITLE}}"
status: proposed
deciders: "{{DECIDERS}}"
date: "{{DATE}}"
---

<!--
================================================================================
GUIA: Architecture Decision Record (ADR)
================================================================================

QUANDO USAR
Use este tipo para registrar decisoes arquiteturais importantes.
Crie um ADR quando:
- Tomar uma decisao tecnica significativa
- Escolher entre alternativas com trade-offs
- Precisar documentar o "por que" de uma escolha

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Usar Stripe para pagamentos")
- status: proposed | accepted | deprecated | superseded
- deciders: Lista de pessoas que participaram da decisao
- date: Data da decisao

RELACIONAMENTOS
- Nasce de: Discussoes em meetings ou necessidades de specs
- Referencia: specs e contexts afetados
- Pode ser superseded por: outro ADR mais recente

DICAS
- Sempre documente pelo menos 2 alternativas consideradas
- Inclua pros/cons de cada alternativa
- Explique claramente por que a alternativa foi rejeitada
- Use voz ativa: "Usaremos X porque Y"

Apague este bloco de comentario ao usar o template.
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
