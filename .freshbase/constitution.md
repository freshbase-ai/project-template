# Project Constitution

> Este documento define os princípios, padrões e fluxos de trabalho que regem este projeto.

## 1. Princípios Fundamentais (Freshbase Spec Standard)

1.  **Contexto antes do Código:** Nenhuma linha de código é escrita sem um entendimento claro do problema de negócio (Discovery) e da solução funcional (Spec).
2.  **Single Source of Truth:** A documentação na pasta `.freshbase` (ou `contexts/`) é a verdade absoluta. Se o código contradiz a doc, o código está errado (ou a doc precisa ser atualizada).
3.  **Rastreabilidade:** Toda Task técnica deve ser rastreável até uma Spec, que deve ser rastreável até um Problema ou Hipótese de negócio.
4.  **Language Ubiquity:** Usamos a mesma terminologia (Domain Language) no código, na documentação e nas conversas.

## 2. Estrutura de Camadas

* **Discovery (Why):** Focada em problemas de negócio, métricas e hipóteses.
* **Product (What):** Focada em requisitos funcionais, user stories e comportamento (BDD).
* **Technical (How):** Focada em implementação, modelos de dados e tarefas.

## 3. Workflow de Desenvolvimento

1.  **Ingestão:** Reuniões e insights são processados em `discovery/`.
2.  **Definição:** Problemas validados viram Specs dentro de seus respectivos `contexts/`.
3.  **Planejamento:** Tech Leads quebram Specs em Plans e Tasks.
4.  **Implementação:** Devs executam Tasks.

## 4. Definição de Pronto (DoD)

Para uma feature ser considerada completa:
- [ ] Spec aprovada pelo Product Owner.
- [ ] Código implementado conforme Plan.
- [ ] Testes (unitários/integração) passando conforme Scenarios.
- [ ] Documentação atualizada.
