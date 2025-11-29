# Complexity Budget Charter

**Project:** [Project Name]  
**Version:** [X.Y]  
**Effective Date:** [YYYY-MM-DD]  
**Approved By:** [Name/Role]

---

## Purpose

Establish acceptable thresholds for cognitive load in user flows and code complexity to prevent accidental complexity accumulation and maintain product quality.

---

## User Flow Complexity Budgets

### Budget Definitions

**Per-Flow Load Budget:** Maximum cognitive load score allowed for a complete user flow  
**Per-Step Load Budget:** Maximum cognitive load score allowed for a single step within a flow

### Standard Budgets by Flow Type

| Flow Type | Total Budget | Per-Step Budget | Justification |
|-----------|--------------|-----------------|---------------|
| Critical Path (e.g., signup, purchase) | 18/30 | 3/10 per step | Must be effortless; users have clear intent |
| Power User Workflows | 24/30 | 5/10 per step | Higher germane load acceptable; users are trained |
| Infrequent Admin Tasks | 20/30 | 4/10 per step | Moderate complexity OK; frequency is low |
| Error Recovery Flows | 15/30 | 3/10 per step | Stress state requires simplicity |

### Custom Flow Budgets

| Flow Name | Total Budget | Per-Step Budget | Rationale | Review Frequency |
|-----------|--------------|-----------------|-----------|------------------|
| [Flow name] | [X/30] | [Y/10] | [Why this budget] | Monthly/Quarterly |

---

## Code Complexity Budgets

### Function-Level Budgets

| Metric | Threshold | Action if Exceeded |
|--------|-----------|-------------------|
| Cyclomatic Complexity | ≤10 | Refactor required before merge |
| Cognitive Complexity | ≤15 | Refactor recommended |
| Max Nesting Depth | ≤4 levels | Mandatory simplification |
| Lines of Code per Function | ≤50 | Split function |
| Parameters per Function | ≤5 | Refactor to parameter object |

### Module-Level Budgets

| Metric | Threshold | Action if Exceeded |
|--------|-----------|-------------------|
| Lines of Code per Module | ≤500 | Decompose module |
| Public API Surface | ≤15 methods | Review interface design |
| Dependencies (Afferent/Efferent) | ≤10 | Reduce coupling |
| Abstraction Layers | ≤5 levels | Flatten hierarchy |

### System-Level Budgets

| Metric | Threshold | Action if Exceeded |
|--------|-----------|-------------------|
| Service Dependencies | ≤12 per service | Review architecture |
| Total Abstractions | ≤[X] for codebase size | Prune unnecessary abstractions |
| Semantic Vocabulary | ≤[X] core concepts | Consolidate terminology |

---

## Load Type Targets

For each flow/module, allocate budget across load types:

### Target Distribution for Critical Flows

```
Intrinsic Load:   40-50% of budget  (unavoidable domain complexity)
Extraneous Load:  0-10% of budget   (minimize noise/friction)
Germane Load:     40-50% of budget  (learning that builds mastery)
```

### Target Distribution for Power User Flows

```
Intrinsic Load:   30-40% of budget
Extraneous Load:  0-5% of budget
Germane Load:     55-65% of budget  (higher productive learning)
```

---

## Budget Enforcement

### Gates

**Design Gate:**
- [ ] Flow complexity estimate documented
- [ ] Budget allocated and justified
- [ ] Load reduction strategies identified if over budget

**Code Review Gate:**
- [ ] Static analysis confirms complexity within thresholds
- [ ] Reviewer validates cognitive load of changes
- [ ] Any budget exceptions documented and approved

**Release Gate:**
- [ ] User flow audits confirm budget compliance
- [ ] Complexity debt documented if budget exceeded
- [ ] Remediation plan exists for over-budget items

### Exception Process

**When to Request Exception:**
- Domain intrinsic complexity genuinely requires higher budget
- Temporary over-budget state during refactoring
- External constraints (APIs, regulations) force complexity

**Exception Request Template:**

| Field | Value |
|-------|-------|
| Flow/Module | [Name] |
| Current Budget | [X] |
| Requested Budget | [Y] |
| Duration | Permanent / Temporary until [Date] |
| Justification | [Detailed explanation] |
| Mitigation Plan | [How to minimize impact] |
| Approved By | [Name/Role] |
| Review Date | [Date] |

---

## Budget Review & Adjustment

### Quarterly Review Process

1. **Analyze Violations:** Count and categorize budget exceedances
2. **Assess Impact:** Review user feedback, support tickets, code quality metrics
3. **Adjust Budgets:** Tighten or relax budgets based on data
4. **Update Charter:** Document changes and rationale

### Triggers for Budget Adjustment

**Tighten Budget When:**
- User confusion or support tickets increasing
- Developer onboarding time increasing
- Bug rate correlates with complexity
- Performance degradation

**Relax Budget When:**
- User sophistication increases (power users)
- Domain inherently complex and cannot be simplified
- Budget causing artificial constraints that harm design

---

## Budget Monitoring Dashboard

### Key Metrics

| Metric | Target | Current | Status | Trend |
|--------|--------|---------|--------|-------|
| % Flows Within Budget | ≥90% | [%] | 🟢/🟡/🔴 | ↗️/→/↘️ |
| % Modules Within Budget | ≥95% | [%] | 🟢/🟡/🔴 | ↗️/→/↘️ |
| Avg Load Score (Critical Flows) | ≤18/30 | [X] | 🟢/🟡/🔴 | ↗️/→/↘️ |
| Avg Cyclomatic Complexity | ≤8 | [X] | 🟢/🟡/🔴 | ↗️/→/↘️ |
| Active Budget Exceptions | ≤5 | [#] | 🟢/🟡/🔴 | ↗️/→/↘️ |

---

## Complexity Debt Tracking

**Over-Budget Items:**

| Item | Type | Current Complexity | Budget | Overage | Priority | Remediation Plan | Owner | Target Date |
|------|------|-------------------|--------|---------|----------|------------------|-------|-------------|
| [Flow/Module] | Flow/Code | [X] | [Y] | [Delta] | 🔴/🟡/🟢 | [Plan] | [Name] | [Date] |

**Complexity Debt Ledger:**
- **Total Debt:** [Sum of all overages]
- **Trend:** Increasing / Stable / Decreasing
- **Target Debt:** [Acceptable threshold]

---

## Best Practices

### Design Phase
- [ ] Estimate complexity before implementation
- [ ] Allocate budget across intrinsic/extraneous/germane
- [ ] Identify simplification opportunities early
- [ ] Use progressive disclosure for high-germane flows

### Implementation Phase
- [ ] Run static analysis continuously
- [ ] Refactor when approaching threshold (don't wait for violation)
- [ ] Extract functions/modules proactively
- [ ] Use linters configured with budget thresholds

### Review Phase
- [ ] Validate complexity during code review
- [ ] Test user flows for cognitive load
- [ ] Update budget tracking dashboard
- [ ] Log exceptions and debt

---

## Appendix: Calculation Methods

### User Flow Load Scoring
[Document your specific scoring methodology - e.g., steps × load factors]

### Code Complexity Measurement Tools
- **Cyclomatic Complexity:** [Tool/command]
- **Cognitive Complexity:** [Tool/command]
- **Static Analysis:** [Tool configuration]

### Load Audit Process
[Reference to Cognitive Load Audit template]

---

**TRACE:** L4:CognitiveLoad:Budget  
**Cross-ref:** Cognitive Load Audit, Psychological Lens (L3), Design Stage (L2), Architectural DNA (L1)
