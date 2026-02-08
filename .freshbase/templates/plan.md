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
GUIA: Plano de Implementacao (Plan)
================================================================================

QUANDO USAR
Use este tipo para planejar a implementacao de uma spec.
Crie um plan quando:
- Uma spec foi aprovada e esta pronta para implementacao
- Precisar quebrar o trabalho em tarefas menores
- Quiser rastrear progresso e dependencias

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Implementacao: One-click Checkout")
- spec: Referencia a spec sendo implementada
- status: planning | in_progress | blocked | completed

CAMPOS OPCIONAIS
- owner: Responsavel pela implementacao
- effort: S | M | L | XL (estimativa de esforco)

RELACIONAMENTOS
- Nasce de: spec aprovada
- Quebra em: tasks/fases de implementacao
- Referencia: ADRs de decisoes tecnicas

DICAS
- Divida em fases logicas (Foundation, Core, Integration)
- Inclua pre-requisitos e dependencias
- Mantenha um log de progresso
- Defina criterios claros de "done"

Apague este bloco de comentario ao usar o template.
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
