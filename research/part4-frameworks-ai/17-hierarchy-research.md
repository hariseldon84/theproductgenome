# Chapter 17: Builder's Hierarchy — Research

**Research Date:** December 2, 2025
**Researcher:** Mary (Business Analyst)
**Status:** Complete

---

## Key Findings

### 1. Impact Mapping (Gojko Adzic)

- **Core purpose**: Creating better plans and roadmaps that ensure **alignment of business and delivery**
- **Problems addressed**:
  - Wrong assumptions
  - Lack of focus
  - Poor communication of objectives
  - Lack of understanding
  - Misalignment with overall goals
- **Value orientation**: Reorients teams towards delivering **value, not delivering features**
- **Strategic planning method**: Simple yet incredibly effective, based on user interaction design, outcome-driven planning, and mind mapping
- **Hierarchy structure**:
  1. **Goal** (Why?): Business objective
  2. **Actors** (Who?): Who can produce desired effect?
  3. **Impacts** (How?): How should actors' behavior change?
  4. **Deliverables** (What?): What can we do to support impacts?
- **Traceability**: Focus on impacts for key actors translates well into outcomes
- **Outcome focus**: Most planning activities revolve around "shopping list of features" — even when delivered, business objective often not achieved
- **Collaborative tool**: Helps teams test mutual understanding of product goals and expected outcomes

### 2. Capability Mapping (TOGAF / Enterprise Architecture)

- **Definition**: Self-contained view of business independent of current organizational structure, processes, IT systems, and products
- **TOGAF Integration**: Business capabilities core feature of TOGAF Standard 10th Edition
- **Mapping relationships**: Capabilities mapped back to:
  - Organizational units
  - Value streams
  - Information systems
  - Strategic plans
- **Alignment insight**: Provides greater insight into alignment and optimization of each domain
- **Capability-Based Planning**: Links to Enterprise Architecture with all architectures expressed in **business outcomes and value** (not IT terms)
- **Corporate strategy driver**: Strategic direction drives Architecture Vision (Phase A), organization creates basis for portfolios
- **Portfolio coordination**: Capability managers perform similar tasks to portfolio managers, aligning projects/increments to deliver continuous business value
- **Phase alignment**: Specific capabilities targeted for completion drive Architecture Definition (Phases B-D), work packages inform Phase E projects

### 3. Hierarchical Decision-Making & Traceability

- **Strategic alignment frameworks**: Ensure features trace back to strategic objectives
- **Hierarchy prevents drift**: Clear levels (outcome → capability → feature → task) maintain strategic connection
- **Decision authority**: Different levels require different decision-making authority
- **Visibility**: Hierarchical structure provides visibility from strategy to execution
- **Portfolio management integration**: Standard practices ensure alignment across initiatives

---

## Sources

### Impact Mapping

1. **[Impact Mapping - Gojko Adzic](https://gojko.net/books/impact-mapping/)**
   - Official book site
   - Core methodology

2. **[Impact Mapping: Making a Big Impact | Official Site](https://www.impactmapping.org/)**
   - Comprehensive resource
   - Templates and guides

3. **[Impact Mapping | Open Practice Library](https://openpracticelibrary.com/practice/impact-mapping/)**
   - Practical application
   - Workshop formats

4. **[Software That Matters: A Review of Impact Mapping | EBG Consulting](https://www.ebgconsulting.com/blog/software-that-matters-a-review-of-gojko-adzics-impact-mapping/)**
   - Critical review
   - Real-world application insights

### Capability Mapping & TOGAF

5. **[TOGAF Business Capability Model: Definitive Guide | KnowledgeHut](https://www.knowledgehut.com/blog/it-service-management/business-capability-modelling)**
   - Comprehensive guide
   - Implementation details

6. **[The TOGAF Standard - Capability-Based Planning](https://pubs.opengroup.org/architecture/togaf9-doc/arch/chap28.html)**
   - Official TOGAF documentation
   - Framework details

7. **[Open Group TOGAF Business Capability](https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html)**
   - Standard definition
   - Best practices

8. **[Comprehensive Guide to Business Capability Planning in TOGAF | Visual Paradigm](https://togaf.visual-paradigm.com/2025/01/21/comprehensive-guide-to-business-capability-planning-in-togaf/)**
   - 2025 updated guide
   - Practical examples

9. **[Business Capabilities Guide | Bizzdesign](https://bizzdesign.com/blog/business-capabilities-a-complete-guide)**
   - Complete framework overview
   - Industry perspectives

---

## Statistics & Data Points

### Impact Mapping Outcomes

- **Hierarchy levels**: 4 (Goal → Actors → Impacts → Deliverables) — [Source 2](https://www.impactmapping.org/)
- **Focus shift**: From "shopping list of features" to outcome-driven planning — [Source 4](https://www.ebgconsulting.com/blog/software-that-matters-a-review-of-gojko-adzics-impact-mapping/)

### TOGAF & Capability Mapping

- **TOGAF 10th Edition**: Business capabilities as core feature — [Source 7](https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html)
- **Mapping dimensions**: 4 (organizational units, value streams, info systems, strategic plans) — [Source 5](https://www.knowledgehut.com/blog/it-service-management/business-capability-modelling)

---

## Case Examples

### Impact Mapping: Software That Matters

- **Context**: Traditional planning creates feature shopping lists
- **Problem**: Features delivered but business objectives not achieved
- **Impact Mapping Solution**:
  - Start with clear business goal
  - Identify actors who can produce desired effect
  - Define behavior change (impact) needed
  - Only then determine deliverables (features)
- **Outcome**: Features connected to business impact, easier to say "no" to non-aligned requests
- **Source**: [EBG Consulting Review](https://www.ebgconsulting.com/blog/software-that-matters-a-review-of-gojko-adzics-impact-mapping/)

### TOGAF Capability Planning: Enterprise Alignment

- **Context**: Large enterprise with multiple IT systems, organizational changes
- **Problem**: IT investments misaligned with business strategy
- **Capability-Based Planning Solution**:
  - Map business capabilities (independent of current org structure)
  - Link capabilities to value streams and strategic plans
  - Coordinate portfolio management around capabilities
  - Phase E projects derived from capability gaps
- **Outcome**: IT expressed in business terms, alignment visibility, continuous value delivery
- **Source**: [TOGAF Capability-Based Planning](https://pubs.opengroup.org/architecture/togaf9-doc/arch/chap28.html)

### Hierarchy Drift Prevention: Spotify Squads (Anti-Pattern)

- **Context**: Autonomous squads empowered to make decisions
- **Problem**: Without clear hierarchy connecting squad work to company strategy, drift occurred
- **Symptom**: Squads building features misaligned with company objectives
- **Lesson**: Autonomy requires hierarchical clarity — squads need to understand where their work fits
- **Source**: Common industry knowledge (Spotify model evolution)

---

## Quotes for Book

> "Impact mapping helps to create better plans and roadmaps that ensure alignment of business and delivery, addressing common problems like wrong assumptions, lack of focus, poor communication of objectives, lack of understanding and misalignment with overall goals."
> — Gojko Adzic, via [Open Practice Library](https://openpracticelibrary.com/practice/impact-mapping/)

> "Impact Mapping reorients us towards delivering value, not delivering features."
> — via [EBG Consulting](https://www.ebgconsulting.com/blog/software-that-matters-a-review-of-gojko-adzics-impact-mapping/)

> "Most planning activities revolve around juggling a 'shopping list of features,' and even though the features are delivered, often the business objective is not achieved."
> — Gojko Adzic, Impact Mapping

> "The business capability map provides a self-contained view of the business that is independent of the current organizational structure, business processes, IT systems and applications, and the product or service portfolio."
> — TOGAF Standard, via [Open Group](https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html)

> "In the TOGAF ADM, business capabilities are mapped back to organizational units, value streams, information systems, and strategic plans, providing greater insight into the alignment and optimizations of each of these domains."
> — via [TOGAF Business Capability](https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html)

> "Capability management is aligned with Enterprise Architecture, with all architectures expressed in terms of business outcomes and value rather than in IT terms, thereby ensuring IT alignment with the business."
> — via [TOGAF Capability-Based Planning](https://pubs.opengroup.org/architecture/togaf9-doc/arch/chap28.html)

> "Capability managers perform similar tasks to portfolio managers, but across the portfolios aligning the projects and project increments to deliver continuous business value."
> — via [TOGAF Documentation](https://pubs.opengroup.org/architecture/togaf9-doc/arch/chap28.html)

---

## Anti-Patterns to Avoid

### 1. Feature Backlog Without Outcome Traceability

- **Pattern**: Backlog full of feature requests with no link to business goals
- **Evidence**: Teams can't answer "why are we building this?" beyond "stakeholder asked for it"
- **Cost**: Wasted capacity on low-value features (80% unused features, Ch 1)
- **Counter**: Impact Mapping — every feature traces to actor impact and business goal

### 2. Capability Mapping Without Refresh

- **Pattern**: Create capability map once, never update as business evolves
- **Evidence**: Capabilities misaligned with current strategy, map becomes shelf-ware
- **Cost**: Planning disconnected from reality, capabilities don't reflect actual business
- **Counter**: Quarterly capability review aligned with strategic planning cycles

### 3. Too Many Hierarchy Levels

- **Pattern**: 7+ levels between strategy and execution (outcomes → themes → epics → capabilities → features → stories → tasks → subtasks)
- **Evidence**: Decision-making paralysis, unclear authority, bureaucracy
- **Cost**: Slow decisions, cognitive load (Ch 15), coordination overhead
- **Counter**: 3-4 levels maximum (Outcomes → Capabilities → Features → Tasks, per Impact Mapping)

### 4. Bottom-Up Hierarchy

- **Pattern**: Define tasks/features first, try to retrofit into capabilities/outcomes later
- **Evidence**: Strategic incoherence, features don't align when rolled up
- **Cost**: "Peanut butter spread" — resources thinly across unaligned initiatives
- **Counter**: Top-down — start with outcome, decompose to capabilities, then features

### 5. No Decision Rights Per Level

- **Pattern**: Unclear who decides at each hierarchy level
- **Evidence**: Every decision escalates, bottlenecks at leadership
- **Cost**: Slow execution, disempowered teams, leadership burnout
- **Counter**: Clear decision authority — outcomes (exec), capabilities (product), features (squad), tasks (eng)

### 6. Hierarchy Without Traceability Tools

- **Pattern**: Hierarchy exists conceptually but not enforced in tools
- **Evidence**: JIRA tickets don't link to strategic objectives, no rollup reporting
- **Cost**: Alignment invisible, can't prove strategic progress
- **Counter**: Tool configuration enforcing hierarchy (epics → stories with mandatory strategic tag)

---

## Cross-References

### Related Chapters

- **Chapter 3 (Feature Factory)**: Builder's Hierarchy prevents output obsession by maintaining outcome connection
- **Chapter 5 (Purpose DNA)**: Top of hierarchy — Purpose defines strategic outcomes
- **Chapter 6 (User DNA)**: Actors in Impact Mapping = User archetypes/segments
- **Chapter 10 (Validation DNA)**: Validate at each level (outcome hypothesis, capability value, feature usage)
- **Chapter 13 (Evolution Flow Cycle)**: Vision → Decompose phase applies Builder's Hierarchy
- **Chapter 21 (Governance by Artifacts)**: Hierarchy documented in artifacts (strategy docs, ADRs, roadmaps)

### Related Frameworks

- **Impact Mapping**: Goal → Actors → Impacts → Deliverables (4-level hierarchy)
- **TOGAF Capability-Based Planning**: Strategy → Capabilities → Projects → Features
- **Evolution Flow Cycle**: Vision (outcome level) → Decompose (capability level) → Design → Build (feature/task level)
- **OKRs**: Objectives (outcomes) → Key Results (capabilities/metrics) → Initiatives (features)

### Related DNAs

- **Purpose DNA**: Defines strategic outcomes (top of hierarchy)
- **User DNA**: Defines actors (Impact Mapping second level)
- **Architecture DNA**: Capabilities often map to architectural modules/bounded contexts
- **Validation DNA**: Validation criteria defined at each hierarchy level
- **Cultural DNA**: Hierarchy clarity reflects value of strategic alignment

---

## Open Questions

1. **Optimal Hierarchy Depth**: Is 4 levels always right, or does it depend on organization size? (Startups vs enterprises)

2. **Capability Lifespan**: How long should capabilities remain stable? (Too stable = inflexible; too dynamic = chaos)

3. **Tool Enforcement**: Should hierarchy be enforced via tools (JIRA/Linear), or is conceptual understanding sufficient?

4. **Cross-Functional Capabilities**: How to model capabilities that span multiple product areas? (Shared services, platforms)

5. **Hierarchy vs Autonomy**: How to balance hierarchical clarity with team autonomy? (Spotify lesson: autonomy without alignment = drift)

6. **Outcome Measurement**: How to measure outcome achievement at each level? (Metrics cascade?)

7. **Portfolio Coordination**: At what organizational scale does capability-based portfolio management become necessary? (10 teams? 50? 100?)

---

## Next Research Steps

1. ✅ Core frameworks identified (Impact Mapping, TOGAF Capability Mapping)
2. ⏭️ **Deeper on OKRs**: How OKRs operationalize hierarchy (Objectives → Key Results → Initiatives)
3. ⏭️ **Wardley Mapping**: Strategic visualization complementing hierarchy
4. ⏭️ **Portfolio management standards**: PMI, SAFe, LeSS approaches to hierarchy
5. ⏭️ **Case studies**: Find examples of hierarchy preventing drift (or failing to prevent)
6. ⏭️ **Tool integration**: How tools like JIRA, Aha!, ProductBoard enforce hierarchy
7. ⏭️ **Bounded contexts**: Domain-Driven Design's strategic design as capability mapping alternative

---

**TRACE:** `RESEARCH:CH17:HIERARCHY:v1.0`
**Last Updated:** December 2, 2025
