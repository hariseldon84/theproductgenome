# Template: Constraint Lens

Purpose: Define guardrails, trade-offs, and safe boundaries for decisions.

## Inputs
- Purpose/Cultural guardrails
- Architecture constraints

## Checks
- Trade-off clarity: speed vs quality; user vs business value
- Safety boundaries: feature flags, rollback, isolation
- Compliance & risk controls

## Outputs (Artifacts)
- Guardrail Charter: explicit do/don’t and conditions
- Trade-off Log: decisions with rationale
- Safety Plan: flags, rollback steps, isolation strategies

## Anti-Patterns
- Toxic urgency; "ship now, fix later"
- Hidden risk acceptance

## Traceability
- `TRACE:L3:Constraint:<section>`

## Ready-to-Use Prompt
```
Goal: Apply Constraint Lens to <decision>
Inputs: guardrails, constraints
Output: guardrail charter + trade-off log + safety plan
```