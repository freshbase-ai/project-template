---
type: hypothesis
title: "{{TITLE}}"
status: draft
problem: "{{PROBLEM_REFERENCE}}"
---

<!--
================================================================================
GUIDE: Solution Hypothesis (Hypothesis)
================================================================================

WHEN TO USE
Use this type to document hypotheses to be validated.
Create a hypothesis when:
- You have a solution idea for a validated problem
- You need to test an assumption before investing in development
- You want to structure a validation experiment

REQUIRED FIELDS
- title: Descriptive name (e.g., "One-click checkout reduces abandonment")
- status: draft | testing | validated | invalidated
- problem: Reference to the problem this hypothesis tries to solve

RELATIONSHIPS
- Born from: problem (the problem being solved)
- Validates through: experiments, A/B tests, prototyping
- If validated, generates: spec (solution specification)

TIPS
- Use the format "We believe... For... Will achieve... We know when..."
- List critical assumptions that must be true
- Define clear success/failure metrics
- Plan experiments with defined timeline

Delete this comment block when using the template.
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

{Results after validation - fill in later}

## Decision

- [ ] Proceed to spec
- [ ] Pivot
- [ ] Abandon
