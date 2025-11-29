# Template: Validate Stage

Purpose: Convert assumptions to evidence; run deterministic gates.

## Inputs
- Test Design Plan
- Experiments (Validation DNA)

## Outputs (Artifacts)
- Test Results: unit/integration/e2e
- Gate Report: PASS/CONCERNS/FAIL with evidence
- Learning Log updates

## Process
- Execute tests; close coverage gaps
- Run QA gate with NFR assessment
- Record learnings and decisions

## Stage Gate
- PASS: All critical ACs covered; NFRs PASS
- CONCERNS: Minor gaps; plan documented
- FAIL: Critical gaps or NFR FAIL

## Anti-Patterns
- Vanity validation
- Skipping gate criteria

## Traceability
- `TRACE:L2:Validate:<section>`

## Ready-to-Use Prompt
```
Goal: Validate <feature>
Inputs: test plan, experiments
Output: test results + gate report + learnings
```