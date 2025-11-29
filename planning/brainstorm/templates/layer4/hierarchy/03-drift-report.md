# Drift Report

**Project:** [Project Name]  
**Report Date:** [YYYY-MM-DD]  
**Review Period:** [Date range]  
**Prepared By:** [Name/Team]

---

## Executive Summary

**Total Items Reviewed:** [Number]  
**Drift Issues Identified:** [Number]  
**Critical Drift (Immediate Action Required):** [Number]  
**Trend:** Improving / Stable / Worsening

**Key Findings:**
- [High-level finding 1]
- [High-level finding 2]

---

## Drift Categories

### 1. Orphaned Features (No Clear Capability/Outcome Link)

| Feature ID | Feature Name | Added Date | Last Modified | Impact | Recommendation |
|------------|--------------|------------|---------------|--------|----------------|
| F-XXX | [Feature name] | [Date] | [Date] | 🔴 High / 🟡 Medium / 🟢 Low | Retire / Repurpose / Link to CAP-XXX |

**Details:**
- **F-XXX: [Feature Name]**
  - **Current State:** [Description of feature and usage]
  - **Why Orphaned:** [Reason for weak/missing upward link]
  - **Usage Data:** [Adoption metrics if available]
  - **Cost:** [Maintenance burden, tech debt]
  - **Recommendation:** [Specific action]
  - **Owner:** [Name]
  - **Priority:** 🔴/🟡/🟢

---

### 2. Capability Bloat (Features Without Outcome Uplift)

| Capability ID | Feature Count | Outcome Contribution | Bloat Score | Action |
|---------------|---------------|---------------------|-------------|--------|
| CAP-XXX | [Count] | Weak/None | 🔴 High / 🟡 Med / 🟢 Low | Prune / Consolidate / Validate |

**Details:**
- **CAP-XXX: [Capability Name]**
  - **Feature List:** [F-001, F-002, F-003...]
  - **Outcome Link:** [OUT-XXX] — Validation Status: [Pass/Fail/Partial]
  - **Problem:** [Description of bloat - too many features, unclear value]
  - **Recommendation:** [Specific action - consolidate, remove redundant, clarify outcome]
  - **Impact if Unchanged:** [Risk description]

---

### 3. Weak Upward Links (Ambiguous Mappings)

| Item | Type | Upstream Link | Issue | Recommendation |
|------|------|---------------|-------|----------------|
| F-XXX | Feature | CAP-XXX → OUT-XXX | Ambiguous/Contested | Clarify / Re-map / Split |

**Details:**
- **F-XXX: [Feature Name]**
  - **Current Mapping:** F-XXX → CAP-XXX → OUT-XXX → [Purpose]
  - **Issue:** [Why link is weak - multiple interpretations, contested ownership, unclear value]
  - **Evidence:** [Stakeholder confusion, conflicting requirements, metrics don't align]
  - **Recommendation:** [Clarify mapping, split feature, consolidate with another]

---

### 4. Outcome Gaps (Missing Capabilities)

| Outcome ID | Outcome Statement | Gap Description | Priority | Proposed Action |
|------------|-------------------|-----------------|----------|-----------------|
| OUT-XXX | [Outcome] | Missing capability: [Description] | 🔴/🟡/🟢 | Add CAP-XXX / Adjust outcome |

**Details:**
- **OUT-XXX: [Outcome Statement]**
  - **Required Capabilities:** [List of capabilities needed]
  - **Current Coverage:** [What exists]
  - **Gap:** [What's missing]
  - **Business Impact:** [Why this matters]
  - **Recommendation:** [Build new capability / adjust outcome scope / deprioritize]

---

### 5. Telemetry Disconnects (Unmeasured Claims)

| Item | Claim | Telemetry Status | Gap | Action |
|------|-------|------------------|-----|--------|
| OUT-XXX | [Outcome claim] | Missing / Insufficient / Wrong metrics | [Description] | Add metric / Fix instrumentation |

**Details:**
- **OUT-XXX: [Outcome Statement]**
  - **Claim:** [What we say we're achieving]
  - **Current Telemetry:** [What we're actually measuring]
  - **Gap:** [Why current metrics don't validate the claim]
  - **Recommendation:** [Add specific instrumentation, change outcome claim, both]

---

## Drift Score Summary

| Category | Items | Critical | Medium | Low | Trend |
|----------|-------|----------|--------|-----|-------|
| Orphaned Features | [#] | [#] | [#] | [#] | ↗️/→/↘️ |
| Capability Bloat | [#] | [#] | [#] | [#] | ↗️/→/↘️ |
| Weak Links | [#] | [#] | [#] | [#] | ↗️/→/↘️ |
| Outcome Gaps | [#] | [#] | [#] | [#] | ↗️/→/↘️ |
| Telemetry Disconnects | [#] | [#] | [#] | [#] | ↗️/→/↘️ |

---

## Corrective Action Plan

### Critical (Immediate - Next Sprint)
1. **[Action]** — Item: [F-XXX/CAP-XXX/OUT-XXX] — Owner: [Name] — Due: [Date]
2. **[Action]** — Item: [ID] — Owner: [Name] — Due: [Date]

### Important (This Quarter)
1. **[Action]** — Item: [ID] — Owner: [Name] — Due: [Date]

### Improvement (Next Quarter)
1. **[Action]** — Item: [ID] — Owner: [Name] — Due: [Date]

---

## Prevention Measures

**Process Improvements:**
- [ ] [Improvement to prevent future drift]
- [ ] [Gate or checklist addition]
- [ ] [Review cadence adjustment]

**Governance:**
- [ ] [Policy or guideline update]
- [ ] [Role/responsibility clarification]

---

## Appendix: Drift Audit Methodology

**Review Process:**
1. Retrieve latest Hierarchy Trace Matrix
2. For each feature, validate capability → outcome → purpose chain
3. Check telemetry coverage for all outcome claims
4. Compare feature list against capability definitions for coherence
5. Score drift severity based on [criteria]

**Scoring Criteria:**
- 🔴 Critical: [Definition]
- 🟡 Medium: [Definition]
- 🟢 Low: [Definition]

---

**TRACE:** L4:Hierarchy:Drift  
**Cross-ref:** Trace Matrix, Capability Health Dashboard, Decomposition Stage (L2)
