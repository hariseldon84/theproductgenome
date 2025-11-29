# Template: Architectural Lens

Purpose: Enforce boundaries, contracts, and observability for evolvable design.

## Inputs
- ADRs, NFRs
- Contracts & dependency map

## Checks
- Boundary integrity: ownership, interface clarity
- Contract adherence: schemas, API signatures
- Observability: logs, metrics, traces

## Outputs (Artifacts)
- Boundary Review: violations + fixes
- Contract Compliance Report
- Observability Checklist

## Anti-Patterns
- Architecture by accident; framework-first decisions
- Missing telemetry or unclear error semantics

## Traceability
- `TRACE:L3:Architectural:<section>`

## Ready-to-Use Prompt
```
Goal: Apply Architectural Lens to <component>
Inputs: ADRs, contracts
Output: boundary review + compliance report + observability checklist
```