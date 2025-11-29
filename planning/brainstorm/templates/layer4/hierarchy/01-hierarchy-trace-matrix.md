# Hierarchy Trace Matrix

**Project:** [Project Name]  
**Date:** [YYYY-MM-DD]  
**Prepared By:** [Name/Team]

---

## Purpose
Map features to capabilities, outcomes, and purpose to ensure upward justification and prevent drift.

---

## Trace Map

| Feature ID | Feature Name | Maps to Capability | Maps to Outcome | Maps to Purpose | Status | Notes |
|------------|--------------|-------------------|-----------------|-----------------|--------|-------|
| F-001 | [Feature name] | [Capability ID/Name] | [Outcome ID/Name] | [Purpose statement] | ✅ Aligned / ⚠️ Weak / ❌ Orphan | [Context/issues] |
| F-002 | | | | | | |
| F-003 | | | | | | |

---

## Capability Coverage Check

| Capability ID | Capability Name | Implementing Features | Outcome Link | Health Score | Notes |
|---------------|-----------------|----------------------|--------------|--------------|-------|
| CAP-001 | [Capability] | [F-001, F-003] | [Outcome ID] | 🟢 Healthy / 🟡 At Risk / 🔴 Failing | [Comments] |
| CAP-002 | | | | | |

---

## Outcome Validation

| Outcome ID | Outcome Statement | Supporting Capabilities | Telemetry Metrics | Validated? | Notes |
|------------|-------------------|------------------------|-------------------|------------|-------|
| OUT-001 | [Measurable outcome] | [CAP-001, CAP-002] | [Metric names] | ✅ Yes / ❌ No / ⏳ Pending | [Evidence/gaps] |
| OUT-002 | | | | | |

---

## Drift Report

**Orphaned Features** (no clear capability/outcome link):
- [ ] F-XXX: [Feature name] — Reason: [Why orphaned]

**Weak Links** (ambiguous or contested mappings):
- [ ] F-XXX → CAP-XXX: [Description of weakness]

**Capability Gaps** (outcomes without sufficient capabilities):
- [ ] OUT-XXX: [Outcome] — Missing: [Required capability]

---

## Action Items

| Priority | Action | Owner | Due Date | Status |
|----------|--------|-------|----------|--------|
| 🔴 High | [Action item] | [Name] | [Date] | Open/In Progress/Done |
| 🟡 Medium | | | | |
| 🟢 Low | | | | |

---

**TRACE:** L4:Hierarchy:Matrix  
**Cross-ref:** Purpose DNA (L1), Architecture DNA (L1), Decomposition Stage (L2)
