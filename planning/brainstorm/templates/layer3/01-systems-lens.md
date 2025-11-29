# Template: Systems Lens

Purpose: Apply holistic system thinking to detect coupling, feedback loops, and flow integrity.

## Inputs
- Component map & interfaces
- Data and control flows

## Checks
- Dependency graph: directionality, cycles, hidden couplings
- Flow integrity: entry/exit criteria, failure modes
- Feedback loops: telemetry → decisions → changes

## Outputs (Artifacts)
- System Map: responsibilities, boundaries, interactions
- Risk Matrix: coupling/flow risks + mitigations
- Observability Plan: metrics/traces for system health

## Anti-Patterns
- Local optimization at expense of system coherence
- Hidden shared state; tight coupling

## Traceability
- `TRACE:L3:Systems:<section>`

## Ready-to-Use Prompt
```
Goal: Apply Systems Lens to <scope>
Inputs: components, flows
Output: system map + risk matrix + observability plan
```