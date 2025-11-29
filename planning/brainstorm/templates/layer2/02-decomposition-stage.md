# Template: Decomposition Stage

Purpose: Break vision into components and atomic work packets aligned to DNAs.

## Inputs
- Vision Brief
- Layer 1 DNAs constraints

## Outputs (Artifacts)
- Component Map: services, UI flows, data entities
- Work Packet List: IDs, descriptions, ACs, dependencies
- Capability Trace: feature → capability → outcome

## Process
- Identify components and seams
- Define packets with ACs and dependencies
- Map packets to Purpose/User/Experience constraints

## Stage Gate
- PASS: Packets are atomic, testable, and aligned
- CONCERNS: Over-sized or unclear dependencies
- FAIL: No trace to outcomes or DNAs

## Anti-Patterns
- Feature bucket lists without ACs
- Ignoring seams and boundaries

## Traceability
- `TRACE:L2:Decomposition:<section>`

## Ready-to-Use Prompt
```
Goal: Decompose <initiative> into components & packets
Inputs: Vision Brief, DNAs
Output: component map + packet list + capability trace
```