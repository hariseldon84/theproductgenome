# Refactor Opportunity Ledger

**Project:** [Project Name]  
**Last Updated:** [YYYY-MM-DD]  
**Maintained By:** [Team/Role]

---

## Purpose

Track identified opportunities to reduce extraneous cognitive load through refactoring, ranked by impact and effort.

---

## Opportunity Scoring

**Impact Score (1-10):**
- 10: Critical user/developer pain, high usage, significant load reduction
- 5: Moderate pain, medium usage
- 1: Minor improvement, low usage

**Effort Score (1-10):**
- 10: Massive refactor, cross-cutting changes, high risk
- 5: Moderate complexity, few dependencies
- 1: Quick fix, isolated change

**Priority = Impact / Effort**  
(Higher ratio = do first)

---

## Refactor Opportunities (Active)

| ID | Opportunity | Type | Impact | Effort | Priority | Status | Owner | Target Date |
|----|-------------|------|--------|--------|----------|--------|-------|-------------|
| REF-001 | [Description] | User/Code | [1-10] | [1-10] | [Ratio] | Queued/In Progress/Done | [Name] | [Date] |
| REF-002 | | | | | | | | |

---

## Opportunity Detail Template

### REF-001: [Short Title]

**Type:** User Flow / Code Module / Both

**Current State:** [Description of current complexity/friction]

**Problem:**
- **Cognitive Load Type:** Extraneous (primary target) / Mislabeled Intrinsic / Under-optimized Germane
- **Specific Issues:**
  - [Issue 1]
  - [Issue 2]
- **Evidence:** [User feedback, support tickets, analytics, code metrics]
- **Affected Users/Developers:** [Count, segments]

**Proposed Refactor:**
[Detailed description of the change]

**Expected Benefits:**
- **Load Reduction:** [Estimate - e.g., "Reduce step load from 7/10 to 3/10"]
- **User Impact:** [What improves for users]
- **Developer Impact:** [What improves for team]
- **Secondary Benefits:** [Performance, maintainability, etc.]

**Scoring:**
- **Impact Score:** [X/10] — Justification: [Why this score]
- **Effort Score:** [Y/10] — Justification: [Why this score]
- **Priority:** [X/Y] = [Ratio]

**Implementation Plan:**
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Risks:**
- [Risk 1] — Mitigation: [Plan]
- [Risk 2] — Mitigation: [Plan]

**Dependencies:**
- Requires: [Other refactors, architectural changes]
- Blocks: [What's waiting on this]

**Success Metrics:**
- [ ] Load score reduced to [target]
- [ ] User complaints/tickets reduced by [%]
- [ ] Code complexity within budget
- [ ] [Other measurable outcome]

**Status:** Queued / In Progress / Done / Deferred

---

### REF-002: [Short Title]

[Repeat structure above]

---

## Completed Refactors (Last 6 Months)

| ID | Title | Completed Date | Actual Impact | Actual Effort | Lessons Learned |
|----|-------|----------------|---------------|---------------|-----------------|
| REF-XXX | [Title] | [Date] | [Score] | [Score] | [Key insights] |

---

## Deferred/Rejected Opportunities

| ID | Title | Reason Deferred/Rejected | Reconsider Date |
|----|-------|--------------------------|-----------------|
| REF-XXX | [Title] | [Why not doing now] | [Date to revisit] |

---

## Refactor by Category

### User Flow Simplification

**Opportunities:**
- REF-001: [Title] — Priority: [X]
- REF-005: [Title] — Priority: [X]

**Total Estimated Load Reduction:** [X points]

---

### Code Complexity Reduction

**Opportunities:**
- REF-002: [Title] — Priority: [X]
- REF-007: [Title] — Priority: [X]

**Total Estimated Complexity Reduction:** [X points]

---

### Semantic Consistency Improvements

**Opportunities:**
- REF-003: [Title] — Priority: [X]
- REF-009: [Title] — Priority: [X]

**Total Terminology Conflicts Resolved:** [X]

---

### Abstraction Simplification

**Opportunities:**
- REF-004: [Title] — Priority: [X]

**Total Abstraction Layers Removed:** [X]

---

## Prioritization Matrix

```
High Impact, Low Effort (DO FIRST)
│ REF-003 │ REF-007 │
├─────────┼─────────┤
│ REF-001 │ REF-002 │
└─────────┴─────────┘
     ↓
Low Impact, High Effort (DO LAST / DEFER)
```

**Quadrant Breakdown:**

| Quadrant | Count | IDs |
|----------|-------|-----|
| High Impact, Low Effort (Quick Wins) | [#] | [REF-XXX, REF-XXX] |
| High Impact, High Effort (Strategic) | [#] | [REF-XXX] |
| Low Impact, Low Effort (Nice-to-Have) | [#] | [REF-XXX] |
| Low Impact, High Effort (Avoid) | [#] | [REF-XXX] |

---

## Sprint/Release Planning

### This Sprint

**Committed Refactors:**
- [ ] REF-XXX: [Title] — Owner: [Name]
- [ ] REF-XXX: [Title] — Owner: [Name]

**Expected Load Reduction:** [X points]

---

### Next Quarter

**Planned Refactors:**
1. REF-XXX: [Title]
2. REF-XXX: [Title]
3. REF-XXX: [Title]

**Expected Cumulative Load Reduction:** [X points]

---

## Refactor Retrospective

### REF-XXX: [Completed Refactor Title]

**Completed:** [Date]

**Outcomes:**
- **Load Reduction:** Estimated [X], Actual [Y]
- **User Impact:** [Measured improvement]
- **Effort:** Estimated [X days], Actual [Y days]

**What Went Well:**
- [Success 1]

**What Could Improve:**
- [Learning 1]

**Reusable Patterns:**
- [Pattern or approach to apply to future refactors]

---

## Metrics Dashboard

| Metric | Target | Current | Trend |
|--------|--------|---------|-------|
| Active Opportunities | [Track growth/decline] | [#] | ↗️/→/↘️ |
| Avg Priority Score | [Baseline] | [X] | ↗️/→/↘️ |
| Refactors Completed (This Quarter) | ≥[X] | [#] | 🟢/🟡/🔴 |
| Total Load Reduction (YTD) | ≥[X] points | [Y] | 🟢/🟡/🔴 |
| Refactor ROI (Impact/Effort actual) | ≥[X] | [Y] | 🟢/🟡/🔴 |

---

## Governance

### Adding New Opportunities

**Trigger Events:**
- Cognitive Load Audit identifies extraneous load
- User complaints/support tickets about confusion
- Code review flags complexity
- Developer onboarding reveals poor clarity

**Submission Template:**
[Link to opportunity detail template above]

### Approval Process

**Minor Refactors (Effort ≤ 3):**
- Team lead approval
- Add to backlog

**Major Refactors (Effort > 3):**
- Architecture review
- Impact assessment
- Resource allocation approval

### Review Cadence

- **Weekly:** New opportunities reviewed and scored
- **Sprint Planning:** Select opportunities for upcoming sprint
- **Quarterly:** Review completed refactors, adjust scoring model

---

## Anti-Patterns to Avoid

- [ ] Refactoring for perfection (diminishing returns)
- [ ] Ignoring high-impact, high-effort opportunities (strategic value)
- [ ] Refactoring without measuring outcomes (validate load reduction)
- [ ] Breaking working code without user/developer benefit

---

**TRACE:** L4:CognitiveLoad:Refactor  
**Cross-ref:** Cognitive Load Audit, Complexity Budget Charter, Architectural DNA (L1), Build Stage (L2)
