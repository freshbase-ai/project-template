# Project Constitution

> This document defines the principles, standards and workflows that govern this project.

## 1. Fundamental Principles (Freshbase Spec Standard)

1.  **Context before Code:** No line of code is written without a clear understanding of the business problem (Discovery) and the functional solution (Spec).
2.  **Single Source of Truth:** The documentation in the `.freshbase` folder (or `contexts/`) is the absolute truth. If the code contradicts the doc, the code is wrong (or the doc needs to be updated).
3.  **Traceability:** Every technical Task must be traceable to a Spec, which must be traceable to a business Problem or Hypothesis.
4.  **Language Ubiquity:** We use the same terminology (Domain Language) in code, documentation, and conversations.

## 2. Layer Structure

* **Discovery (Why):** Focused on business problems, metrics, and hypotheses.
* **Product (What):** Focused on functional requirements, user stories, and behavior (BDD).
* **Technical (How):** Focused on implementation, data models, and tasks.

## 3. Development Workflow

1.  **Ingestion:** Meetings and insights are processed in `discovery/`.
2.  **Definition:** Validated problems become Specs within their respective `contexts/`.
3.  **Planning:** Tech Leads break down Specs into Plans and Tasks.
4.  **Implementation:** Devs execute Tasks.

## 4. Definition of Done (DoD)

For a feature to be considered complete:
- [ ] Spec approved by the Product Owner.
- [ ] Code implemented according to Plan.
- [ ] Tests (unit/integration) passing according to Scenarios.
- [ ] Documentation updated.
