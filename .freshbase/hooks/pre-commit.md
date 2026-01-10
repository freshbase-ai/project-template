# Pre-Commit Verification

Before committing documentation, verify:

- [ ] Documentation is in **Markdown** (.md)
- [ ] No sensitive information (tokens, passwords, personal data)
- [ ] Files are organized in the correct folders
- [ ] FSS templates were followed when applicable
- [ ] Internal links are working (use `[[wiki-links]]`)
- [ ] Commit message is descriptive and follows the pattern `docs: <description>`

## FSS v1.0 Structure

- `overview/` - Project overview, glossary, data-flows
- `flows/` - Cross-cutting business flows
- `contexts/` - DDD bounded contexts
- `discovery/` - Problems and hypotheses
- `features/` - BDD feature specifications
- `specs/` - Technical specifications
- `decisions/` - Architecture Decision Records (ADRs)
- `meetings/` - Meeting transcriptions and notes
- `cross-cutting/` - Cross-context features
- `uncategorized/` - Documents not yet organized

## Checklist by Document Type

### Spec (Specification)
- [ ] Is in the correct location (`specs/` or `contexts/{domain}/specs/`)
- [ ] References the problem in `discovery/problems/`
- [ ] Has user stories and acceptance criteria

### ADR (Decision Record)
- [ ] Is in `decisions/`
- [ ] Has defined status (Proposed/Accepted/Deprecated)
- [ ] Documents alternatives considered

### Meeting Notes
- [ ] Is in `meetings/`
- [ ] Has date and participants
- [ ] Lists extracted actions

### Flows (flows/*.md)
- [ ] All involved modules are listed
- [ ] Main flow (happy path) is documented
- [ ] Error scenarios have recovery actions
- [ ] Links to related contexts and specs

### Context (contexts/*.md)
- [ ] Has clear boundary definition
- [ ] Includes domain language/glossary
- [ ] Lists key features and responsibilities
