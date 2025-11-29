# APAP Template: Prompt Decomposition Map

Purpose: Break down a high-level vision into atomic, testable work packets aligned to DNA and gates.

## Inputs
- Vision statement
- Core user outcomes
- Constraints (time, budget, compliance)

## Decomposition Grid

| Track | Outcome | Constraints | Risks | DNA Alignment | Lens | References |
|------|---------|-------------|-------|---------------|------|------------|
| Vision → Components |  |  |  |  | Systems |  |
| Frontend |  |  |  |  | Psychological |  |
| Data/Schema |  |  |  |  | Architectural |  |
| Process/Backend |  |  |  |  | Evolution |  |
| Integrations |  |  |  |  | Constraint |  |

## Work Packets
- Packet ID: `APAP-VIS-###`
- Description:
- Acceptance criteria:
- Dependencies:
- DNA gates: Purpose, User, Experience, Architecture, Data, Validation, Growth, Cultural

## Traceability
- Tag each packet with `TRACE:{layer}:{section}`
- Link to ADRs, MQB decisions

## Anti-Patterns Checklist
- Over-specifying prompts
- Ignoring constraints
- Unbounded scope creep

## Ready-to-Generate Prompt
```
Context: <vision + constraints>
Goal: <explicit component/page/service>
Steps: <numbered actions>
Contracts: <APIs, schemas>
Boundaries: <files allowed to change>
Validation: <tests/gates>
```