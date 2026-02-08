---
type: scenarios
title: "{{TITLE}}"
feature: "{{FEATURE_REFERENCE}}"
---

<!--
================================================================================
GUIA: Cenarios BDD (Scenarios)
================================================================================

QUANDO USAR
Use este tipo para documentar cenarios de teste em formato BDD.
Crie scenarios quando:
- Uma spec precisa de criterios de aceitacao detalhados
- Quiser definir comportamento esperado de forma executavel
- Precisar alinhar QA, dev e produto sobre o que "pronto" significa

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Login com email e senha")
- feature: Referencia a spec/feature sendo testada

RELACIONAMENTOS
- Nasce de: spec (criterios de aceitacao)
- Valida: comportamento da implementacao
- Pode virar: testes automatizados

DICAS
- Use formato Given/When/Then consistentemente
- Agrupe cenarios relacionados
- Inclua edge cases e cenarios de erro
- Use Examples para data-driven scenarios

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# {{TITLE}}

**Feature:** [[specs/{{FEATURE}}]]

---

## Scenario Group: {User Story or Capability}

### Scenario: {Descriptive Name}

**Given** {precondition}
**When** {action}
**Then** {expected outcome}

**Examples:**

| {variable1} | {variable2} | {expected} |
|-------------|-------------|------------|
| {value}     | {value}     | {value}    |

---

### Scenario: {Another Scenario}

**Given** {precondition}
  **And** {additional precondition}
**When** {action}
**Then** {expected outcome}
  **And** {additional outcome}

---

## Edge Cases

### Scenario: {Edge Case Name}

**Given** {unusual precondition}
**When** {action}
**Then** {graceful handling}

---

## Error Scenarios

### Scenario: {Error Condition}

**Given** {precondition that leads to error}
**When** {action}
**Then** {error handling behavior}
  **And** {user feedback}
