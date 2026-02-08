---
type: problem
title: "{{TITLE}}"
status: draft
owner: "{{OWNER}}"
source: meeting
---

<!--
================================================================================
GUIA: Problema de Negocio (Problem)
================================================================================

QUANDO USAR
Use este tipo para documentar problemas de negocio identificados.
Crie um problem quando:
- Identificar uma dor do usuario ou gap no produto
- Receber feedback consistente de stakeholders/usuarios
- Detectar metricas negativas ou tendencias preocupantes

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Usuarios abandonam checkout")
- status: draft | validated | invalidated

CAMPOS OPCIONAIS
- owner: Stakeholder responsavel
- source: meeting | interview | analytics | support-ticket

RELACIONAMENTOS
- Nasce de: meetings, entrevistas, analise de dados
- Gera: hypotheses (para validar solucoes)
- Eventualmente leva a: specs (se hipotese validada)

DICAS
- Descreva o problema do ponto de vista do usuario
- Inclua evidencias qualitativas E quantitativas
- Nao proponha solucoes aqui - isso e para hypotheses

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# {{TITLE}}

## Problem Statement

### Who is affected?

{Persona ou grupo de usuarios afetados}

### What is the problem?

{Descricao clara do problema observado}

### Where/When does it occur?

{Contexto em que o problema se manifesta}

### Why does it matter?

{Impacto no negocio/usuario}

## Evidence

### Qualitative

- {Citacao de reuniao/entrevista}
- {Feedback de usuario}

### Quantitative

- {Metrica atual}: {valor}
- {Metrica de suporte}: {valor}

## Context & Relationships

- **Impacted Contexts:** [[contexts/{{CONTEXT}}]]
- **Meetings:** [[meetings/{{DATE}}-{{TITLE}}]]
- **Hypotheses:** [[discovery/hypotheses/HYP-XXX]]

## Notes

{Observacoes adicionais}
