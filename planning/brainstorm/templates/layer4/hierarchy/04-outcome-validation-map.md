# Outcome Validation Map

**Project:** [Project Name]  
**Validation Date:** [YYYY-MM-DD]  
**Review Period:** [Date range]

---

## Purpose
Verify that outcome claims are measurable, instrumented, and validated by telemetry data.

---

## Outcome Registry

| Outcome ID | Outcome Statement | Success Criteria | Target Value | Validation Method |
|------------|-------------------|------------------|--------------|-------------------|
| OUT-001 | [Measurable outcome claim] | [Specific criteria] | [Quantifiable target] | Telemetry / User research / A/B test |
| OUT-002 | | | | |

---

## Outcome Validation Detail

### OUT-001: [Outcome Statement]

**Description:** [Full description of what success looks like]

**Supporting Capabilities:**
- CAP-001: [Capability name]
- CAP-002: [Capability name]

**Success Criteria:**
1. [Criterion 1] — Target: [Value] — Weight: [%]
2. [Criterion 2] — Target: [Value] — Weight: [%]
3. [Criterion 3] — Target: [Value] — Weight: [%]

**Telemetry Instrumentation:**

| Metric Name | Metric Type | Data Source | Collection Method | Current Value | Target | Status |
|-------------|-------------|-------------|-------------------|---------------|--------|--------|
| [Metric] | Frequency/Ratio/Count | [System/Service] | [How measured] | [Value] | [Target] | ✅/⚠️/❌ |
| [Metric] | | | | | | |

**Validation Logic:**
```
IF [Metric A] >= [Target] AND [Metric B] < [Threshold] THEN Outcome = Achieved
ELSE IF [Conditions] THEN Outcome = Partial
ELSE Outcome = Not Achieved
```

**Current Assessment:**
- **Status:** ✅ Achieved / ⚠️ Partial / ❌ Not Achieved / ⏳ Insufficient Data
- **Score:** [X%] of target
- **Evidence:** [Link to dashboard, data summary]
- **Last Validated:** [Date]

**Telemetry Gaps:**
- [ ] [Missing metric or instrumentation]
- [ ] [Data quality issue]

**Corrective Actions (if not achieved):**
1. [Action] — Owner: [Name] — Due: [Date]

---

### OUT-002: [Outcome Statement]

[Repeat structure above]

---

## Validation Dashboard Summary

| Outcome | Status | Score | Trend | Last Validated | Next Review |
|---------|--------|-------|-------|----------------|-------------|
| OUT-001 | ✅ | 95% | ↗️ | [Date] | [Date] |
| OUT-002 | ⚠️ | 67% | → | [Date] | [Date] |
| OUT-003 | ❌ | 32% | ↘️ | [Date] | [Date] |
| OUT-004 | ⏳ | N/A | - | [Date] | [Date] |

---

## Validation Health Check

**Overall Outcome Validation Score:** [X%]

**Breakdown:**
- Fully Validated (✅): [#] outcomes ([%])
- Partially Validated (⚠️): [#] outcomes ([%])
- Not Validated (❌): [#] outcomes ([%])
- Insufficient Data (⏳): [#] outcomes ([%])

**Trends:**
- Improving: [List outcome IDs]
- Declining: [List outcome IDs]
- New outcomes pending instrumentation: [List]

---

## Telemetry Coverage Analysis

### Well-Instrumented Outcomes
[List outcomes with complete telemetry]

### Telemetry Gaps

| Outcome | Missing Metric | Priority | Remediation Plan | Owner | Due Date |
|---------|----------------|----------|------------------|-------|----------|
| OUT-XXX | [Metric name] | 🔴/🟡/🟢 | [Plan] | [Name] | [Date] |

---

## Vanity Metric Warning

**Metrics to Retire/Replace:**

| Current Metric | Problem | Recommended Alternative | Outcome Link |
|----------------|---------|------------------------|--------------|
| [Metric] | [Why it's vanity - measures activity not outcome] | [Better metric] | OUT-XXX |

**Examples of Vanity Metrics:**
- Page views without engagement depth
- Feature usage without outcome contribution
- Sign-ups without activation or retention

---

## Validation Cadence

**Real-time Validation:**
- [List outcomes tracked in real-time dashboards]

**Weekly Review:**
- [List outcomes reviewed weekly]

**Monthly Deep Dive:**
- [List outcomes requiring monthly analysis]

**Quarterly Audit:**
- [Comprehensive validation review process]

---

## Action Items

### Immediate (🔴)
1. **[Action]** — Outcome: OUT-XXX — Owner: [Name] — Due: [Date]

### This Quarter (🟡)
1. **[Action]** — Outcome: OUT-XXX — Owner: [Name] — Due: [Date]

### Future (🟢)
1. **[Action]** — Outcome: OUT-XXX — Owner: [Name] — Due: [Date]

---

## Appendix: Validation Principles

**Good Outcome Validation:**
- Measures results, not activity
- Quantifiable with clear thresholds
- Timely (data available when needed)
- Actionable (informs decisions)
- Tied to user/business value

**Red Flags:**
- Outcome claim without any metrics
- Metrics that can be "gamed"
- Metrics that measure team activity instead of user/business outcomes
- Stale data (more than [X] days old)

---

**TRACE:** L4:Hierarchy:Validation  
**Cross-ref:** Data DNA (L1), Validation DNA (L1), Capability Health Dashboard, Validate Stage (L2)
