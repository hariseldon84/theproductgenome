# Cognitive Load Audit

**Project/Feature:** [Name]  
**Audit Date:** [YYYY-MM-DD]  
**Auditor:** [Name/Team]  
**Scope:** User Flow / Code Module / Full Product

---

## Executive Summary

**Audit Scope:** [Description]  
**Overall Load Score:** [X/100] — 🟢 Manageable / 🟡 High / 🔴 Excessive  
**Primary Load Type:** Intrinsic / Extraneous / Germane

**Key Findings:**
- [Finding 1]
- [Finding 2]
- [Finding 3]

**Immediate Actions Required:** [Count]

---

## Load Classification Framework

**Intrinsic Load:** Inherent complexity of the domain/task (cannot be eliminated)  
**Extraneous Load:** Unnecessary friction, noise, poor design (should be minimized)  
**Germane Load:** Productive cognitive effort that builds understanding (optimize for mastery)

---

## User Flow Cognitive Load Analysis

### Flow: [Flow Name - e.g., "User Onboarding"]

**Flow Steps:**

| Step | Description | Intrinsic Load | Extraneous Load | Germane Load | Total Load | Issues |
|------|-------------|----------------|-----------------|--------------|------------|--------|
| 1 | [Step description] | 🟢 Low / 🟡 Med / 🔴 High | 🟢/🟡/🔴 | 🟢/🟡/🔴 | [Score/10] | [List issues] |
| 2 | | | | | | |
| 3 | | | | | | |

**Flow Load Breakdown:**

```
Total Intrinsic:  [X/10] ████████░░  [Acceptable/High]
Total Extraneous: [X/10] ███░░░░░░░  [Target: minimize]
Total Germane:    [X/10] ██████░░░░  [Optimize]
──────────────────────────────────────
Combined Load:    [X/30] [Status]
```

**Load Budget:** [X/30] — Status: Within/Approaching/Exceeding budget

---

## Detailed Step Analysis

### Step 1: [Step Name]

**User Action:** [What user needs to do]

**Intrinsic Load Assessment:** 🟢 Low
- **Domain Concepts Required:** [List concepts]
- **Complexity Justification:** [Why this complexity is unavoidable]
- **Reducible?** Yes/No — [Explanation]

**Extraneous Load Assessment:** 🔴 High
- **Friction Points:**
  - [ ] Poor labeling/terminology — Example: [Specific issue]
  - [ ] Inconsistent patterns — Example: [Specific issue]
  - [ ] Context switching — Example: [Specific issue]
  - [ ] Unclear navigation — Example: [Specific issue]
  - [ ] Visual clutter — Example: [Specific issue]
  - [ ] Ambiguous states — Example: [Specific issue]
  - [ ] Excessive options — Example: [Specific issue]
  - [ ] Other: [Describe]

**Germane Load Assessment:** 🟡 Medium
- **Learning Opportunity:** [What valuable understanding does this build?]
- **Optimization Potential:** [How to make learning more effective]
- **Retention Aid:** [Progressive disclosure, tooltips, examples used?]

**Specific Issues:**
1. **Issue:** [Description of cognitive burden]
   - **Type:** Extraneous / Mislabeled intrinsic / Under-optimized germane
   - **Impact:** High/Medium/Low
   - **Evidence:** [User confusion, support tickets, analytics]
   - **Recommendation:** [Specific fix]

**Load Score:** [X/10]

---

### Step 2: [Step Name]

[Repeat structure above]

---

## Code Module Cognitive Load Analysis

### Module: [Module Name - e.g., "PaymentService"]

**Module Complexity:**

| Dimension | Score | Status | Notes |
|-----------|-------|--------|-------|
| Cyclomatic Complexity | [Value] | 🟢/🟡/🔴 | Target: <10 per function |
| Abstraction Levels | [Count] | 🟢/🟡/🔴 | Too many nested layers? |
| Naming Consistency | [Score/10] | 🟢/🟡/🔴 | Semantic clarity |
| Coupling | [Score/10] | 🟢/🟡/🔴 | External dependencies |
| Documentation | [Score/10] | 🟢/🟡/🔴 | Code self-documentation |

**Intrinsic Complexity:**
- **Domain Logic:** [Assessment of inherent business rule complexity]
- **Algorithm Complexity:** [Assessment of computational complexity]
- **Reducible?** [Can domain be simplified without losing value?]

**Extraneous Complexity:**
- [ ] Inconsistent naming conventions
- [ ] Unnecessary abstractions (over-engineering)
- [ ] Poor separation of concerns
- [ ] Magic numbers/strings
- [ ] Unclear state management
- [ ] Hidden dependencies
- [ ] Comments explaining "what" instead of "why"

**Germane Complexity:**
- **Learning Curve for New Developers:** [Assessment]
- **Abstraction Value:** [Do abstractions aid understanding or obscure?]
- **Pattern Consistency:** [Does it follow established patterns?]

**Refactoring Opportunities:**
1. [Specific refactoring suggestion] — Impact: [High/Med/Low]

---

## Cognitive Load Budget

### User Flow Budgets

| Flow | Target Load | Current Load | Status | Priority |
|------|-------------|--------------|--------|----------|
| [Flow name] | [X/30] | [Y/30] | Within/Over budget | 🔴/🟡/🟢 |

### Code Module Budgets

| Module | Target Complexity | Current Complexity | Status | Priority |
|--------|-------------------|-------------------|--------|----------|
| [Module name] | [Threshold] | [Value] | Within/Over | 🔴/🟡/🟢 |

---

## Semantic Consistency Analysis

**Terminology Audit:**

| Concept | UI Label | API Name | Code Variable | Documentation Term | Consistency? | Fix Required |
|---------|----------|----------|---------------|-------------------|--------------|--------------|
| [Concept] | [Term] | [Term] | [Term] | [Term] | ✅ Yes / ❌ No | [Action] |

**Inconsistency Issues:**
1. **Concept:** [Concept name]
   - **Variations Found:** [List all terms used]
   - **Impact:** [Confusion it causes]
   - **Recommended Canonical Term:** [Term]
   - **Scope of Change:** [Where to apply]

---

## Context Switching Analysis

**User Context Switches:**

| Flow | Switch Count | Justified? | Avoidable Switches | Recommendation |
|------|--------------|------------|-------------------|----------------|
| [Flow] | [#] | Some/All/None | [#] | [Action] |

**Examples:**
- Switch from [Context A] to [Context B] — Reason: [Why] — Avoidable? [Yes/No]

---

## Attention Economics

**User Attention Budget:**
- **Critical Path Focus:** [What requires deep attention?]
- **Peripheral Elements:** [What's competing for attention?]
- **Attention Waste:** [Distractions, unnecessary elements]

**Recommendations:**
- [ ] Remove/hide: [Element]
- [ ] Prioritize: [Element]
- [ ] Defer/progressive disclosure: [Element]

---

## Action Plan

### Immediate (🔴 High Impact, Quick Win)
1. **[Action]** — Flow/Module: [Name] — Load Reduction: [Estimate] — Owner: [Name] — Due: [Date]
2. **[Action]** — Flow/Module: [Name] — Load Reduction: [Estimate] — Owner: [Name] — Due: [Date]

### This Sprint/Quarter (🟡 Important)
1. **[Action]** — Flow/Module: [Name] — Load Reduction: [Estimate] — Owner: [Name] — Due: [Date]

### Future Improvements (🟢 Optimization)
1. **[Action]** — Flow/Module: [Name] — Load Reduction: [Estimate] — Owner: [Name] — Due: [Date]

---

## Validation & Re-Audit

**Success Criteria:**
- [ ] Extraneous load reduced by [X%]
- [ ] User flow load score below [threshold]
- [ ] Code complexity within budget
- [ ] Semantic consistency at [X%]

**Next Audit Date:** [Date]

---

**TRACE:** L4:CognitiveLoad:Audit  
**Cross-ref:** Experience DNA (L1), Psychological Lens (L3), Design Stage (L2), Complexity Budget Charter
