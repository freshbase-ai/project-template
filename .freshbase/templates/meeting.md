---
type: meeting
title: "{{TITLE}}"
date: "{{DATE}}"
participants: []
duration: 0
source: manual
---

<!--
================================================================================
GUIA: Notas de Reuniao (Meeting)
================================================================================

QUANDO USAR
Use este tipo para documentar reunioes e suas decisoes.
Crie um meeting quando:
- Tiver uma reuniao importante (discovery, refinement, review)
- Receber uma transcricao de Fireflies/Otter
- Precisar registrar decisoes e action items

CAMPOS OBRIGATORIOS
- title: Nome descritivo (ex: "Sprint 32 Planning")
- date: Data da reuniao (YYYY-MM-DD)

CAMPOS OPCIONAIS
- participants: Lista de participantes
- duration: Duracao em minutos
- source: fireflies | manual | otter | zoom

RELACIONAMENTOS
- Gera: problems, hypotheses, specs, ADRs (extraidos da reuniao)
- Referencia: specs e contexts discutidos

DICAS
- Extraia action items com owners e deadlines
- Identifique problemas e hipoteses mencionados
- Use o collapsible para transcricao completa
- Mantenha o summary conciso (2-3 frases)

Apague este bloco de comentario ao usar o template.
================================================================================
-->

# {{TITLE}}

## Summary

{2-3 frases resumindo o objetivo e resultado da reuniao}

## Key Decisions

1. {decision-1} - **Owner:** {name}
2. {decision-2} - **Owner:** {name}

## Action Items

- [ ] {action-1} - **Owner:** {name} | **Due:** {date}
- [ ] {action-2} - **Owner:** {name} | **Due:** {date}

## Insights

### Problems Identified

- [[discovery/problems/PRB-XXX]]: {brief description}

### Requirements Discussed

- {requirement-1}
- {requirement-2}

### Open Questions

- {question-1} - **Needs:** {who can answer}

## Raw Notes / Transcript

<details>
<summary>Expand transcript</summary>

{transcricao completa ou notas detalhadas}

</details>
