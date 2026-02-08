---
type: hypothesis
title: "{{TITLE}}"
status: draft
problem: "{{PROBLEM_REFERENCE}}"
---

<!--
================================================================================
GUIA: Hipotese de Solucao (Hypothesis)
================================================================================

QUANDO USAR
Use este tipo para documentar hipoteses a serem validadas.
Crie uma hypothesis quando:
- Tiver uma ideia de solucao para um problema validado
- Precisar testar uma suposicao antes de investir em desenvolvimento
- Quiser estruturar um experimento de validacao

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "One-click checkout reduz abandono")
- status: draft | testing | validated | invalidated
- problem: Referencia ao problema que esta hipotese tenta resolver

RELACIONAMENTOS
- Nasce de: problem (problema que esta resolvendo)
- Valida atraves de: experimentos, testes A/B, prototipagem
- Se validada, gera: spec (especificacao da solucao)

DICAS
- Use o formato "We believe... For... Will achieve... We know when..."
- Liste assumptions criticas que devem ser verdadeiras
- Defina metricas claras de sucesso/fracasso
- Planeje experimentos com timeline definido

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# {{TITLE}}

**Problem:** [[discovery/problems/{{PROBLEM}}]]

## Hypothesis Statement

> We believe that {proposed solution/change}
> For {target users/personas}
> Will achieve {expected outcome}
> We will know this is true when {measurable signal}

## Assumptions

### Critical (must be true)

- [ ] {assumption-1}
- [ ] {assumption-2}

### Important (should be true)

- [ ] {assumption-3}

## Validation Plan

### Experiments

1. {experiment-description}
   - **Metric:** {what to measure}
   - **Target:** {success threshold}
   - **Timeline:** {duration}

## Results

{Resultados apos validacao - preencher depois}

## Decision

- [ ] Proceed to spec
- [ ] Pivot
- [ ] Abandon
