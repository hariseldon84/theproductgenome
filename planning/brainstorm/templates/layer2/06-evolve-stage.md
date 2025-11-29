# Template: Evolve Stage

Purpose: Learn, refactor, and plan the next iteration based on evidence.

## Inputs
- Gate Report & Learning Log
- Telemetry & cohort insights

## Outputs (Artifacts)
- Refactor Plan: debts, drift corrections, ADR updates
- Next Iteration Brief: scoped adjustments
- Monitoring Additions: new metrics/alerts

## Process
- Identify changes driven by evidence
- Plan refactors with isolation and tests
- Update ADRs and monitoring

## Stage Gate
- PASS: Evidence-driven changes planned
- CONCERNS: Partial plan or unclear impacts
- FAIL: No evidence linkage or unbounded changes

## Anti-Patterns
- Evolve by opinion
- Deferred debts without rationale

## Traceability
- `TRACE:L2:Evolve:<section>`

## Ready-to-Use Prompt
```
Goal: Evolve <system/feature>
Inputs: gate report, telemetry
Output: refactor plan + iteration brief + monitoring updates
```