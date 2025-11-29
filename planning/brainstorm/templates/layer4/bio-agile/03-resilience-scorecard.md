# Resilience Scorecard

**System/Product:** [Name]  
**Assessment Date:** [YYYY-MM-DD]  
**Assessed By:** [Team/Role]

---

## Purpose

Measure the product's ability to withstand shocks, adapt to stress, and recover from failures using biological resilience principles.

---

## Resilience Framework

**Biological Resilience = Resistance + Recovery + Adaptation**

1. **Resistance:** Ability to withstand stress without degradation
2. **Recovery:** Speed and completeness of bounce-back after shock
3. **Adaptation:** Learning and improving from stressors
4. **Redundancy:** Backup systems and fallback options
5. **Diversity:** Multiple pathways to achieve outcomes

---

## Resilience Assessment

### 1. Technical Resilience

**Infrastructure Robustness:**
| Component | Resistance | Recovery | Adaptation | Score |
|-----------|-----------|----------|------------|-------|
| **Compute/Servers** | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 | [X/10] |
| **Database** | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 | [X/10] |
| **API Services** | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 | [X/10] |
| **Frontend/CDN** | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 | [X/10] |
| **Integrations** | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 | [X/10] |

**Scoring:**
- **Resistance:** Can system handle 2x load? Graceful degradation? (🟢 Yes / 🟡 Partial / 🔴 No)
- **Recovery:** Auto-healing? RTO < 1 hour? (🟢 <15 min / 🟡 <1 hr / 🔴 >1 hr)
- **Adaptation:** Learns from incidents? Auto-scaling? (🟢 Yes / 🟡 Partial / 🔴 No)

**Overall Technical Resilience:** [Average/10]

---

### 2. Operational Resilience

**Incident Response:**
| Capability | Maturity | Evidence | Score |
|------------|----------|----------|-------|
| **Monitoring & Alerting** | 🟢🟡🔴 | [Coverage %, alert quality] | [X/10] |
| **Incident Runbooks** | 🟢🟡🔴 | [% scenarios covered] | [X/10] |
| **On-Call Rotation** | 🟢🟡🔴 | [Coverage, response time] | [X/10] |
| **Post-Mortem Process** | 🟢🟡🔴 | [% incidents with PM, action completion rate] | [X/10] |
| **Communication Plan** | 🟢🟡🔴 | [Internal/external comm speed] | [X/10] |

**Maturity Levels:**
- 🟢 **High:** Proactive, automated, well-documented
- 🟡 **Medium:** Reactive, partially automated
- 🔴 **Low:** Ad-hoc, manual

**Overall Operational Resilience:** [Average/10]

---

### 3. Product Resilience

**Feature Fallback:**
| Feature | Primary Path | Fallback Options | Degradation Grace | Score |
|---------|-------------|------------------|-------------------|-------|
| [Feature 1] | [Description] | [Alt paths] | 🟢🟡🔴 | [X/10] |

**Scoring:**
- **Fallback Options:** Multiple ways to achieve outcome? (🟢 ≥2 / 🟡 1 / 🔴 0)
- **Degradation Grace:** Can users still get value if feature degrades? (🟢 Yes / 🟡 Partial / 🔴 Blocked)

**User Experience Continuity:**
- **Offline Mode:** 🟢 Functional / 🟡 Limited / 🔴 None
- **Progressive Enhancement:** 🟢 Works on all browsers/devices / 🟡 Most / 🔴 Brittle
- **Error Messaging:** 🟢 Clear, actionable / 🟡 Generic / 🔴 Confusing

**Overall Product Resilience:** [Average/10]

---

### 4. Data Resilience

**Data Protection:**
| Mechanism | Implementation | Testing Frequency | Last Test | Score |
|-----------|----------------|-------------------|-----------|-------|
| **Backups** | [Strategy] | [Frequency] | [Date] | [X/10] |
| **Replication** | [Multi-region?] | [Frequency] | [Date] | [X/10] |
| **Disaster Recovery** | [RPO/RTO] | [Frequency] | [Date] | [X/10] |
| **Data Validation** | [Integrity checks] | [Frequency] | [Date] | [X/10] |

**Scoring:**
- **Backups:** Automated, tested, retained appropriately (🟢 All / 🟡 Partial / 🔴 Missing)
- **Replication:** Real-time, multi-region (🟢 Yes / 🟡 Delayed / 🔴 None)
- **DR:** Tested recently, meets RTO/RPO (🟢 <6 mo / 🟡 <1 yr / 🔴 >1 yr)
- **Validation:** Automated checks, corruption detection (🟢 Continuous / 🟡 Periodic / 🔴 None)

**Overall Data Resilience:** [Average/10]

---

### 5. Business Resilience

**Revenue Diversification:**
| Revenue Stream | % Total Revenue | Customer Concentration | Risk |
|----------------|----------------|------------------------|------|
| [Stream 1] | [X]% | Top 10 customers = [Y]% | 🟢🟡🔴 |

**Scoring:**
- 🟢 **Low Risk:** <30% from one stream, <20% from top 10 customers
- 🟡 **Medium Risk:** 30-60% from one stream, 20-40% from top 10
- 🔴 **High Risk:** >60% from one stream, >40% from top 10

**Supplier/Partner Resilience:**
| Dependency | Criticality | Alternatives | Switching Cost | Risk |
|------------|------------|--------------|----------------|------|
| [Vendor/Partner] | High/Med/Low | [# alternatives] | High/Med/Low | 🟢🟡🔴 |

**Scoring:**
- 🟢 **Low Risk:** Multiple alternatives, low switching cost
- 🟡 **Medium Risk:** 1-2 alternatives, medium switching cost
- 🔴 **High Risk:** Single source, high switching cost

**Overall Business Resilience:** [Average/10]

---

### 6. Team Resilience

**Knowledge Distribution:**
| Critical Capability | Bus Factor | Documentation | Training | Risk |
|--------------------|-----------|---------------|----------|------|
| [Capability 1] | [# people] | 🟢🟡🔴 | 🟢🟡🔴 | 🟢🟡🔴 |

**Scoring:**
- **Bus Factor:** (🟢 ≥3 / 🟡 2 / 🔴 1 person knows critical capability)
- **Documentation:** (🟢 Current, comprehensive / 🟡 Outdated / 🔴 Missing)
- **Training:** (🟢 Regular cross-training / 🟡 Ad-hoc / 🔴 None)

**Team Capacity Buffer:**
- Available capacity for incidents: [X]% of team time
- 🟢 **Healthy:** >20% buffer
- 🟡 **Stretched:** 10-20% buffer
- 🔴 **Fragile:** <10% buffer

**Overall Team Resilience:** [Average/10]

---

## Resilience Score Summary

| Dimension | Score | Status | Weight | Contribution |
|-----------|-------|--------|--------|--------------|
| Technical | [X/10] | 🟢🟡🔴 | 25% | [Y] |
| Operational | [X/10] | 🟢🟡🔴 | 20% | [Y] |
| Product | [X/10] | 🟢🟡🔴 | 20% | [Y] |
| Data | [X/10] | 🟢🟡🔴 | 15% | [Y] |
| Business | [X/10] | 🟢🟡🔴 | 10% | [Y] |
| Team | [X/10] | 🟢🟡🔴 | 10% | [Y] |

**Overall Resilience Score:** [Weighted average/10]

**Resilience Rating:**
- 🟢 **High (≥8):** Can withstand major shocks, quick recovery, learning system
- 🟡 **Moderate (5-7):** Some fragility, slower recovery, partial adaptation
- 🔴 **Low (≤4):** Brittle, cascading failures, slow/incomplete recovery

---

## Stress Testing Results

**Recent Stress Events:**
| Date | Event Type | Severity | Response Time | Recovery Time | Adapted? | Lessons |
|------|-----------|----------|---------------|---------------|----------|---------|
| [Date] | [Incident type] | High/Med/Low | [Duration] | [Duration] | Y/N | [Summary] |

**Planned Resilience Tests:**
| Test Type | Frequency | Last Test | Next Test | Pass/Fail |
|-----------|-----------|-----------|-----------|-----------|
| **Load Testing** | [Quarterly] | [Date] | [Date] | [P/F] |
| **Chaos Engineering** | [Monthly] | [Date] | [Date] | [P/F] |
| **DR Drill** | [Annually] | [Date] | [Date] | [P/F] |
| **Security Pentest** | [Annually] | [Date] | [Date] | [P/F] |

---

## Single Points of Failure (SPOF)

| SPOF | Impact if Failed | Mitigation | Priority | Status |
|------|-----------------|------------|----------|--------|
| [Component/Process] | [Cascading effect] | [Plan to eliminate] | 🔴🟡🟢 | Open/Mitigated |

**Example:**
- **SPOF:** Only one person knows deployment process
- **Impact:** Can't ship hotfixes if they're unavailable
- **Mitigation:** Document process, cross-train 2 more engineers
- **Priority:** 🔴 High
- **Status:** In Progress

---

## Redundancy & Diversity Assessment

**System Redundancy:**
| Component | Redundancy Level | Failover Tested | Notes |
|-----------|------------------|----------------|-------|
| [Component] | Active-active / Active-passive / None | 🟢 Recently / 🟡 Stale / 🔴 Never | [Details] |

**Pathway Diversity (Multiple ways to achieve outcomes):**
| Outcome | Primary Path | Alternative Paths | User Awareness |
|---------|-------------|-------------------|----------------|
| [Outcome] | [Path A] | [Path B, Path C] | High / Medium / Low |

**Diversity Score:** [X/10] (Higher = more alternative pathways)

---

## Adaptation & Learning

**Post-Incident Actions:**
- Total incidents (last quarter): [N]
- Post-mortems conducted: [N]
- Action items created: [N]
- Action items completed: [N]
- **Completion Rate:** [X]%

**Completion Rate Health:**
- 🟢 **High:** >80% completion
- 🟡 **Medium:** 50-80% completion
- 🔴 **Low:** <50% completion

**Adaptive Improvements Implemented:**
1. [Improvement from incident A] — Impact: [Description]
2. [Improvement from incident B] — Impact: [Description]

**Learning Culture:** 🟢 Blameless, iterative / 🟡 Defensive / 🔴 Blame-focused

---

## Resilience Investment ROI

**Resilience Initiatives:**
| Initiative | Cost | Benefit | Status | ROI |
|------------|------|---------|--------|-----|
| [Initiative 1] | [$X] | [Downtime avoided, incidents prevented] | Done/In Progress | [Positive/Negative] |

**Example:**
- **Initiative:** Implement chaos engineering
- **Cost:** $50K (tooling + 2 eng-months)
- **Benefit:** Prevented 3 major outages (est. $200K in lost revenue/reputation)
- **Status:** Done
- **ROI:** +$150K positive

---

## Competitive Resilience Comparison

| Competitor | Uptime (%) | MTTR | Public Incidents (last yr) | Perceived Resilience |
|------------|-----------|------|---------------------------|---------------------|
| [Competitor A] | [99.X%] | [X min] | [N] | 🟢🟡🔴 |
| **Us** | [99.X%] | [X min] | [N] | 🟢🟡🔴 |

**Where We Lead:**
- [Dimension]

**Where We Lag:**
- [Dimension] — **Action:** [Plan]

---

## Action Plan

### Critical (🔴)
1. **[Action]** — Dimension: [Name] — Impact: [Estimate] — Owner: [Name] — Due: [Date]

### Important (🟡)
1. **[Action]** — Dimension: [Name] — Impact: [Estimate] — Owner: [Name] — Due: [Date]

### Optimization (🟢)
1. **[Action]** — Dimension: [Name] — Impact: [Estimate] — Owner: [Name] — Due: [Date]

---

## Review Cadence

- **Weekly:** Monitor incidents, MTTR, uptime
- **Monthly:** Stress test results, SPOF mitigation progress
- **Quarterly:** Full resilience audit, competitive comparison
- **Annually:** Major resilience investments, disaster recovery test

---

**TRACE:** L4:BioAgile:Resilience  
**Cross-ref:** Entropy Management Plan, Architectural DNA (L1), Build Stage (L2), Systems Lens (L3)
