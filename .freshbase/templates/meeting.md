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
GUIDE: Meeting Notes (Meeting)
================================================================================

WHEN TO USE
Use this type to document meetings and their decisions.
Create a meeting when:
- You have an important meeting (discovery, refinement, review)
- You receive a transcription from Fireflies/Otter
- You need to record decisions and action items

REQUIRED FIELDS
- title: Descriptive name (e.g., "Sprint 32 Planning")
- date: Meeting date (YYYY-MM-DD)

OPTIONAL FIELDS
- participants: List of participants
- duration: Duration in minutes
- source: fireflies | manual | otter | zoom

RELATIONSHIPS
- Generates: problems, hypotheses, specs, ADRs (extracted from meeting)
- References: discussed specs and contexts

TIPS
- Extract action items with owners and deadlines
- Identify mentioned problems and hypotheses
- Use collapsible for full transcription
- Keep the summary concise (2-3 sentences)

Delete this comment block when using the template.
================================================================================
-->

# {{TITLE}}

## Summary

{2-3 sentences summarizing the meeting objective and outcome}

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

{full transcription or detailed notes}

</details>
