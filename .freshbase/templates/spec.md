---
type: spec
title: "{{TITLE}}"
context: "{{CONTEXT}}"
status: draft
version: "0.1"
---

<!--
================================================================================
GUIA: Especificacao Tecnica (Spec)
================================================================================

QUANDO USAR
Use este tipo para documentar requisitos tecnicos de uma funcionalidade.
Crie uma spec quando:
- Voce tem uma funcionalidade validada (problema + hipotese confirmados)
- Precisa detalhar o "o que" antes do "como"
- Quer alinhar expectativas entre produto e engenharia

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Autenticacao com OAuth 2.0")
- context: Bounded context relacionado (ex: "identity")
- status: draft | in_review | approved | implemented
- version: Versionamento semantico (0.1, 1.0, etc.)

RELACIONAMENTOS
- Nasce de: problem.md ou hypothesis.md
- Gera: plan.md (implementacao) e scenarios.md (testes BDD)
- Referencia: context.md (bounded context) e adr.md (decisoes tecnicas)

DICAS
- Foque no "o que", nao no "como" (isso vai no plan.md)
- Inclua criterios de aceitacao mensuraveis
- Link para documentos relacionados com [[wiki-style]]
- Reference problemas de discovery/problems/

Apague este bloco de comentario ao usar o template.
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
