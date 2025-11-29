# Layer 2: Evolution Flow Cycle

> Navigation: [Session Overview](./00-session-overview.md) · [Layer 1: 8 DNAs](./layer1_dna.md) · [Layer 2 (This)](./layer2_dna.md) · [Layer 3: Builder's Lenses](./layer3_dna.md) · [Layer 4: Extended Frameworks](./layer4_frameworks.md) · [20-Chapter Mapping](./20-chapter-structure-mapping.md)

Vision → Decomposition → Design → Build → Validate → Evolve

This document defines a practical, repeatable operating cycle that turns Layer 1 DNAs into day-to-day execution. Each stage includes inputs, activities, outputs, anti-patterns, and architect’s notes. The cycle is iterative—evidence at Validate informs Evolve, which reshapes Vision.

> Templates: [Layer 2 (Evolution Flow) Templates](./templates/layer2/)

---

## 1. Vision

Purpose-aligned intent and outcomes definition.

**Inputs**
- Layer 1 references: Purpose DNA (problem, outcomes, USP), Cultural DNA (values hierarchy)
- Market/user insights and strategic constraints
- Known guardrails and anti-goals

**Activities**
- Craft a one-page Vision Brief emphasizing outcomes over outputs
- Frame the problem and stakes; define “who benefits and how”
- Set success signals (leading indicators before lagging metrics)
- Identify explicit non-goals to prevent scope creep

**Outputs (Artifacts)**
- Vision Brief (1-page: problem, outcomes, USP, guardrails)
- Outcome Map (measurable states tied to Purpose outcomes)
- Guardrails Register (anti-goals with rationale)

**Anti-Patterns**
- Feature lists disguised as vision
- Ambiguous success (“we’ll know it when we see it”)
- Tool-centric aspirations (framework-first thinking)

**Architect’s Notes**
- Vision must invalidate tempting but misaligned work; if it cannot, strengthen Purpose.
- Favor outcome indicators that can be observed early; avoid vanity metrics.

---

## 2. Decomposition

Break vision into coherent, testable slices across Experience, Architecture, and Data.

**Inputs**
- Vision Brief, Outcome Map, Guardrails
- User DNA (JTBD flows, triggers, constraints)
- Experience DNA MQB and relevant NFR thresholds from Architecture DNA

**Activities**
- Create Story Maps and JTBD Flow Maps from intent → action → outcome
- Identify architectural seams and ownership boundaries; draft ADR seeds
- Enumerate riskiest assumptions; start a Risk Register
- Surface MQB impacts and NFRs for each slice before design/build

**Outputs (Artifacts)**
- Story Map / JTBD Flow Map (slices with entry/exit criteria)
- ADR Seeds (anticipated structural decisions needing documentation)
- Risk Register (assumptions, probability, impact, mitigations)

**Anti-Patterns**
- Slicing by UI screens rather than user outcomes
- Hidden coupling (unclear ownership, shared mutable state)
- Ignoring NFRs until late-stage performance triage

**Architect’s Notes**
- Prefer seams where contracts are explicit (APIs, events).
- Decompose around outcomes and failure isolation, not convenience.

---

## 3. Design

Converge on experience, architecture, and data designs that meet MQB and DNAs.

**Inputs**
- Story/JTBD slices, ADR seeds, Risk Register
- Experience DNA MQB, Interaction Patterns Library
- Architecture DNA principles (modularity, contracts, observability)
- Data DNA instrumentation needs and ontology

**Activities**
- Specify Golden Paths for each slice with MQB acceptance gates
- Define interface contracts (request/response schemas, error semantics)
- Design telemetry: events → metrics → decisions (traceability)
- Plan tests (unit/integration/e2e) and validation experiments up front

**Outputs (Artifacts)**
- Golden Path Specs (flows, budgets, feedback semantics)
- Interface Contracts / API Sketches (including error and latency budgets)
- Instrumentation Plan (event names, payloads, context metadata)
- Test & Experiment Plans (what to validate, how, success thresholds)

**Anti-Patterns**
- Pixel-perfect mockups without MQB, latency, or error semantics
- Contract-less integration (“we’ll fix it in code reviews”)
- Telemetry afterthoughts (events bolted on post-build)

**Architect’s Notes**
- Treat latency/error semantics as binding contracts between design and code.
- Tests are design artifacts; write them as specifications first.

---

## 4. Build

Implement in small, observable increments that respect boundaries and contracts.

**Inputs**
- Golden Path Specs, Interface Contracts, Instrumentation Plan
- Test & Experiment Plans, ADR seeds

**Activities**
- Build slice-first with test-first (critical paths covered before UI polish)
- Keep dependencies directional; inject infrastructure behind domain interfaces
- Add observability hooks per plan (logs, metrics, tracing)
- Link commits to specs/ADRs; maintain change notes

**Outputs (Artifacts)**
- Passing tests (unit/integration/e2e where applicable)
- Telemetry implemented (events flowing to dashboards)
- ADRs updated from seeds to decisions (context, alternatives, consequences)

**Anti-Patterns**
- Big-bang merges; long-lived branches with hidden drift
- Coupling across boundaries “for speed”
- Skipping tests/telemetry under deadline pressure

**Architect’s Notes**
- Make the right thing easy (templates, helpers); the wrong thing hard (checks).
- Small PRs with clear diff rationale reduce risk and speed review.

---

## 5. Validate

Convert assumptions into evidence; enforce MQB and NFR gates before scaling.

**Inputs**
- Implemented slices with telemetry
- Test & Experiment Plans
- MQB and NFR thresholds

**Activities**
- Run experiments: hypothesis → method → threshold → result → decision
- Check MQB gates (performance, accessibility, reliability) programmatically
- Review cohort and flow metrics (activation, retention) for target segments
- Document learnings and pivot triggers when thresholds are missed

**Outputs (Artifacts)**
- Experiment Sheets (design, results, decisions)
- MQB/NFR Gate Reports (pass/fail, remediation items)
- Cohort/Flow Dashboards (activation, retention, error rates)

**Anti-Patterns**
- Confirmation bias (selective data to “prove” assumptions)
- Declaring success without cohort retention or NFR compliance
- Shipping features as “experiments” without falsifiable hypotheses

**Architect’s Notes**
- Invalidation is progress; early failure saves months of waste.
- Validate behavior and economics (unit economics, support burden), not clicks alone.

---

## 6. Evolve

Refine, retire, or scale based on evidence; feed learning back into Vision.

**Inputs**
- Gate reports, experiment results, dashboards
- ADRs and change notes

**Activities**
- Refactor where contracts or performance require (guided by telemetry)
- Deprecate features/paths that fail to meet outcomes; simplify
- Update ADRs, standards, and docs; capture “why,” not just “what”
- Adjust roadmap and Vision Brief to reflect learnings

**Outputs (Artifacts)**
- Change Logs and Deprecation Notes (impact, migration guidance)
- Updated ADRs and Standards (patterns, thresholds)
- Roadmap Adjustments and refreshed Vision Brief

**Anti-Patterns**
- Ossification (“we always do it this way”) blocking adaptation
- Scaling broken hypotheses (premature optimization)
- Documentation rot (decisions made but never recorded)

**Architect’s Notes**
- Culture compounds through documented decisions; make rationale first-class.
- Evolve toward simplicity; complexity must earn its place.

---

## Operating Principles

- Always trace decisions back to Layer 1 DNAs (Purpose, User, Experience, Architecture, Data, Validation, Growth, Cultural)
- Prefer small, testable increments with explicit contracts and telemetry
- Evidence over assumptions at every stage; gates protect quality
- Culture governs trade-offs under pressure; values show up in pixels and code

## Stage Checklists (Quick Use)

**Vision**: Outcomes defined • Non-goals listed • Success signals set

**Decomposition**: Slices by outcomes • Seams identified • Risks logged • MQB/NFR noted

**Design**: Golden paths with budgets • Contracts written • Instrumentation planned • Tests/experiments designed

**Build**: Tests first • Boundaries respected • Telemetry added • ADRs updated

**Validate**: Experiments run • Gates enforced • Cohorts reviewed • Learnings logged

**Evolve**: Refactor/retire/scale • Docs updated • Roadmap adjusted • Vision refreshed

## Cross-References

- Layer 1: `layer1_dna.md`
- Session: `00-session-overview.md`
