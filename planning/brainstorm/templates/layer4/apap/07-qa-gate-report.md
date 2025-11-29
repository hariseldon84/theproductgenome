# APAP Template: QA Gate Report

Purpose: Summarize quality status with deterministic criteria.

## Context
- Story/Feature:
- Scope:
- Reviewer:
- Date:

## Decision
- Gate: PASS | CONCERNS | FAIL | WAIVED
- Status reason (1-2 sentences):

## Evidence
- Tests reviewed: count
- Risks identified: count
- Trace:
  - AC covered: [ ]
  - AC gaps: [ ]

## NFR Validation
- Security: PASS | CONCERNS | FAIL
- Performance: PASS | CONCERNS | FAIL
- Reliability: PASS | CONCERNS | FAIL
- Maintainability: PASS | CONCERNS | FAIL

## Top Issues
- ID / severity / finding / action

## Recommendations
- Immediate:
- Future:

## Ready-to-Generate Prompt
```
Goal: Produce QA gate report for <feature>
Apply deterministic rules
Output: decision + evidence + recommendations
```