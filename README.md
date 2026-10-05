# System Design Lab

A structured personal learning hub for system design, adopting a unified **Docs-as-Code** approach to manage architecture documentation, diagrams, schemas, and test harnesses under version control.

## Design Philosophy

- **Docs-as-Code**: All architecture, contracts, and test specs live alongside code in Git.
- **Visuals via Mermaid.js**: Embedded natively in Markdown for High-Level Design (HLD), Low-Level Design (LLD), Database ERDs, Sequence Flows, and FSM State Machines.
- **API Specs & Test Harnesses via Bruno**: Git-native `.bru` collections for REST/gRPC endpoints and integration scenarios.
- **Formal Contracts**: OpenAPI 3.1 (`.yaml`) or Protobuf (`.proto`) for interface definitions.

---

## Projects Index

| Project | Description | Status |
| :--- | :--- | :--- |

---

## Repository Structure

- `template/`: Blueprint directory used when creating new system design projects.
- `projects/`: Individual system design studies, each containing requirements, estimations, Mermaid diagrams, API contracts, and Bruno test collections.
- `GLOSSARY.md`: Shared system design terminology and mental models.
- `AGENTS.md`: Instructions for AI assistants collaborating in this repository.
