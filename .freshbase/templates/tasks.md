---
title: "{{TITLE}}"
plan: "{{PLAN_REFERENCE}}"
---

<!--
================================================================================
GUIA: Lista de Tarefas (Tasks)
================================================================================

QUANDO USAR
Use este template para detalhar tarefas de um plano de implementacao.
Crie um tasks quando:
- Um plan.md precisa de breakdown mais granular
- Quer rastrear progresso de tarefas individuais
- Precisa paralelizar trabalho entre membros da equipe

CAMPOS SUGERIDOS
- title: Nome descritivo (ex: "Tasks: One-click Checkout")
- plan: Referencia ao plano pai

RELACIONAMENTOS
- Nasce de: plan.md (plano de implementacao)
- Detalha: fases e tarefas do plano
- Rastreia: progresso individual

DICAS
- Marque tarefas paralelas com [P]
- Inclua checkpoints ao final de cada fase
- Mantenha estimativas de esforco
- Atualize status conforme progresso

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# Tasks: {{TITLE}}

**Plan:** [[plans/{{PLAN}}]]
**Total Tasks:** {count}
**Status:** {X}/{Y} complete

---

## Phase 1: Foundation

### 1.1 {Task Title}

- **File(s):** `{path/to/file}`
- **Dependencies:** None | {task-id}
- **Parallel:** [P] (se pode rodar em paralelo)
- **Estimate:** {hours}
- [ ] {subtask-1}
- [ ] {subtask-2}

### 1.2 {Task Title}

- **File(s):** `{path/to/file}`
- **Dependencies:** 1.1
- [ ] {subtask-1}

**Checkpoint:** {What should be working after Phase 1}

---

## Phase 2: Core Implementation

### 2.1 {Task Title} [P]

- **User Story:** US-001
- **File(s):** `{path}`
- **Dependencies:** 1.2
- [ ] {subtask}

### 2.2 {Task Title} [P]

- **User Story:** US-001
- **File(s):** `{path}`
- **Dependencies:** 1.2
- [ ] {subtask}

**Checkpoint:** {What should be working after Phase 2}

---

## Phase 3: Tests & Integration

### 3.1 Unit Tests

- **File(s):** `tests/unit/`
- **Dependencies:** 2.x
- [ ] Tests for {component-1}
- [ ] Tests for {component-2}

### 3.2 Integration Tests

- **File(s):** `tests/integration/`
- **Dependencies:** 3.1
- [ ] E2E for {flow-1}

**Checkpoint:** All tests passing

---

## Summary

| Phase | Tasks | Status |
|-------|-------|--------|
| Foundation | {X} | pending |
| Core | {X} | pending |
| Tests | {X} | pending |
