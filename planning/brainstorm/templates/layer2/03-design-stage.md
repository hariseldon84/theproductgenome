# Template: Design Stage

Purpose: Specify interfaces, flows, states, and constraints (MQB, NFRs).

## Inputs
- Component Map & Packets
- MQB Charter & UX SLAs (Layer 1)
- Architecture ADRs & NFRs (Layer 1)

## Outputs (Artifacts)
- Interface Contracts: API signatures, schemas, events
- Flow Specs: golden paths, state transitions, error semantics
- Test Design Plan: unit/integration/e2e scope & priorities

## Process
- Define contracts and schemas
- Diagram flows and states (loading/empty/error/success)
- Choose test levels per requirement (unit first mindset)

## Stage Gate
- PASS: Contracts complete, flows clear, tests planned
- CONCERNS: Partial contracts or missing error semantics
- FAIL: No MQB/NFR alignment or test plan

## Anti-Patterns
- Screen-first without flows
- Unspecified error behaviors

## Traceability
- `TRACE:L2:Design:<section>`

## Ready-to-Use Prompt
```
Goal: Design interfaces & flows for <component>
Inputs: packets, MQB, ADRs
Output: contracts, flow specs, test design plan
```