---
type: scenarios
title: "{{TITLE}}"
feature: "{{FEATURE_REFERENCE}}"
---

<!--
================================================================================
GUIDE: BDD Scenarios (Scenarios)
================================================================================

WHEN TO USE
Use this type to document test scenarios in BDD format.
Create scenarios when:
- A spec needs detailed acceptance criteria
- You want to define expected behavior in an executable way
- You need to align QA, dev, and product on what "done" means

REQUIRED FIELDS
- title: Descriptive name (e.g., "Login with email and password")
- feature: Reference to the spec/feature being tested

RELATIONSHIPS
- Born from: spec (acceptance criteria)
- Validates: implementation behavior
- Can become: automated tests

TIPS
- Use Given/When/Then format consistently
- Group related scenarios
- Include edge cases and error scenarios
- Use Examples for data-driven scenarios

Delete this comment block when using the template.
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
