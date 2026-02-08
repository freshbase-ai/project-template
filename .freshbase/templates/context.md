---
type: context
title: "{{CONTEXT_NAME}}"
responsibility: "{{RESPONSIBILITY}}"
---

<!--
================================================================================
GUIA: Bounded Context (Context)
================================================================================

QUANDO USAR
Use este tipo para definir bounded contexts (DDD).
Crie um context quando:
- Identificar um subdominio distinto no sistema
- Precisar definir fronteiras claras de responsabilidade
- Quiser estabelecer a linguagem ubiqua do dominio

CAMPOS OBRIGATORIOS
- title: Nome do bounded context (ex: "Identity & Authentication")
- responsibility: Resumo da responsabilidade principal

RELACIONAMENTOS
- Contem: specs (funcionalidades do contexto)
- Referencia: ADRs sobre decisoes do contexto
- Relaciona-se com: outros contexts (upstream/downstream)

DICAS
- Defina claramente o que o contexto FAZ e NAO FAZ
- Crie um glossario com a linguagem do dominio
- Minimize dependencias entre contexts
- Use Anti-Corruption Layers para integracao externa

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# {{CONTEXT_NAME}}

> **Definition:** What this bounded context does and DOES NOT do.

## Responsibility

**This context IS responsible for:**
- ...

**This context IS NOT responsible for:**
- ...

## Domain Language

| Term | Definition |
|------|------------|
| _Example Term_ | _Clear definition in business language_ |

## Key Features

- [[specs/{{FEATURE}}/spec.md]]

## Dependencies

### Upstream (this context depends on)

- None

### Downstream (depends on this context)

- None

## Integration Points

| System | Direction | Protocol | Notes |
|--------|-----------|----------|-------|
| _External API_ | _Inbound_ | _REST_ | _Description_ |

## Related

- ADRs: [[decisions/ADR-XXX]]
- Flows: [[flows/{{FLOW}}]]
