# FSS Documentation Style Guide

## Language

- Use **Portuguese (pt-BR)** for all documentation
- Maintain terminological consistency (define glossary per context)
- Domain terms must be defined in each context's `context.md`

## Writing Principles

1. **Clarity over Conciseness**: Clear documentation > short documentation
2. **Actionable**: Every specification must have acceptance criteria
3. **Contextualized**: Documents belong to a bounded context
4. **Versionable**: Use Git to track evolution

## Project Structure

### Standard Layout

```
project/
├── overview/           # Macro view
│   ├── README.md      # Executive overview
│   ├── glossary.md    # Domain terms
│   └── data-flows.md  # Module interactions
├── flows/             # Cross-cutting flows
│   ├── onboarding.md
│   └── cancellation.md
├── contexts/          # DDD bounded contexts
├── discovery/         # Problems and hypotheses
├── features/          # BDD specifications
├── specs/             # Technical specifications
├── decisions/         # ADRs
├── meetings/          # Meeting notes
└── .freshbase/        # Configuration
```

### When to create a flow/

- Process involves 2+ modules
- There is orchestration between systems
- There are defined states and transitions

## FSS v1.0 Structure

### Document Hierarchy

```
Discovery (Why?) → Context (What?) → Spec (How?) → Plan (When?)
```

### Workflow

1. **Problem** → Identify and document in `discovery/problems/`
2. **Hypothesis** → Formulate in `discovery/hypotheses/`
3. **Context** → Define bounded context in `contexts/`
4. **Spec** → Detail requirements in `specs/`
5. **Plan** → Create implementation plan

## Document Formats

### Context (DDD Context)
```markdown
# Context: {Name}
> Definition: What it DOES and DOES NOT do

## Domain Language
| Term | Definition |
```

### Spec (Specification)
```markdown
# Spec: {Name}
Ref: [[discovery/problems/{id}]]

## User Stories
## Functional Requirements
## Acceptance Criteria
```

### BDD Scenarios
```gherkin
Feature: [Name]

Scenario: [Description]
  Given [context]
  When [action]
  Then [result]
```

## Commit Messages

Format: `docs(<context>): <description>`

**Scopes:**
- `discovery`: Problems, hypotheses, meetings
- `context/{name}`: Specifications for a context
- `adr`: Architectural decisions
- `cross-cutting`: Cross-cutting features

**Examples:**
```
docs(discovery): document checkout performance problem
docs(context/payments): add spec for automatic refund
docs(adr): record decision about processing queue
```

## Internal Links

Use wiki-links for cross-references:

```markdown
[[discovery/problems/001-slow-checkout]]
[[contexts/payments/specs/automatic-refund]]
[[decisions/adr-003-redis-queue]]
```
