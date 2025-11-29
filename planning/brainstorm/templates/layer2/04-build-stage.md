# Template: Build Stage

Purpose: Implement with boundaries, contracts, observability, and safety.

## Inputs
- Contracts & Flow Specs
- Test Design Plan

## Outputs (Artifacts)
- Implementations: code, configs
- Observability: logs, metrics, traces
- Dependency Map: imports through approved boundaries

## Process
- Implement following contracts (no deviation without ADR)
- Add telemetry and error handling
- Keep dependencies centralized (e.g., `deps.ts`)

## Stage Gate
- PASS: Contract adherence, telemetry wired, boundaries respected
- CONCERNS: Minor drift or missing observability
- FAIL: Broken contracts or unsafe dependencies

## Anti-Patterns
- Hidden dependencies
- Ad-hoc error handling

## Traceability
- `TRACE:L2:Build:<section>`

## Ready-to-Use Prompt
```
Goal: Build <component/service>
Inputs: contracts, flow specs, test plan
Output: code + observability + dependency map
```