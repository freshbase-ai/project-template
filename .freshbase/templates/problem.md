---
type: problem
title: "{{TITLE}}"
status: draft
owner: "{{OWNER}}"
source: meeting
---

<!--
================================================================================
GUIDE: Business Problem (Problem)
================================================================================

WHEN TO USE
Use this type to document identified business problems.
Create a problem when:
- Identifying a user pain point or product gap
- Receiving consistent feedback from stakeholders/users
- Detecting negative metrics or concerning trends

REQUIRED FIELDS
- title: Descriptive name (e.g., "Users abandon checkout")
- status: draft | validated | invalidated

OPTIONAL FIELDS
- owner: Responsible stakeholder
- source: meeting | interview | analytics | support-ticket

RELATIONSHIPS
- Born from: meetings, interviews, data analysis
- Generates: hypotheses (to validate solutions)
- Eventually leads to: specs (if hypothesis validated)

TIPS
- Describe the problem from the user's point of view
- Include qualitative AND quantitative evidence
- Don't propose solutions here - that's for hypotheses

Delete this comment block when using the template.
================================================================================
-->

# {{TITLE}}

## Problem Statement

### Who is affected?

{Persona or group of affected users}

### What is the problem?

{Clear description of the observed problem}

### Where/When does it occur?

{Context in which the problem manifests}

### Why does it matter?

{Business/user impact}

## Evidence

### Qualitative

- {Quote from meeting/interview}
- {User feedback}

### Quantitative

- {Current metric}: {value}
- {Support metric}: {value}

## Context & Relationships

- **Impacted Contexts:** [[contexts/{{CONTEXT}}]]
- **Meetings:** [[meetings/{{DATE}}-{{TITLE}}]]
- **Hypotheses:** [[discovery/hypotheses/HYP-XXX]]

## Notes

{Additional observations}
