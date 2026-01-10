# Features

BDD feature specifications using Gherkin format.

## Structure

Each feature is a `.feature` file or markdown with Gherkin scenarios:

- `user-authentication.feature`
- `checkout-flow.feature`

## Template

```gherkin
# language: pt
@feature:name @tag
Funcionalidade: [Title]
  Como [User Role]
  Quero [Action/Goal]
  Para [Business Value]

  Cenário: [Scenario Title]
    Dado que [initial state]
    Quando [user action]
    Então [expected outcome]
```

## Guidelines

- Group related scenarios in one file
- Use tags for categorization (@mvp, @api, @ui)
- Keep scenarios independent
- Use Background for common setup
