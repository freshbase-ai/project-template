# Scenarios: {FEATURE-TITLE}

## Metadata
- **Feature:** [[contexts/{context}/specs/{feature-id}/spec.md]]
- **Updated:** {date}

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
