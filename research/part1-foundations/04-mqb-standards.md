# Chapter 4: Minimum Quality Bar (MQB) & Gates — Research

**Research Date:** November 30, 2025
**Researcher:** Mary (Business Analyst)
**Status:** In Progress

---

## Key Findings

### 1. Definition of Done (DoD) — Agile Quality Standard
- **DoD = Agreed-upon set of items** that must be completed before project/user story considered complete
- **High-level criteria** for determining if product increment is complete
- **Applies to ALL product increments** — defines overall quality of product
- **Includes**: Code quality, testing, documentation, integration
- **Comprehensive checklist**: Functionality, performance, security, compliance, and other necessary standards
- **Quality gate for product increment** (vs acceptance criteria = quality gate for user story)
- **Collaborative creation**: Entire team (sometimes multiple teams or whole product organization)
- **Purpose**: Ensures uniform quality and completeness across entire product development

### 2. Acceptance Criteria — Feature-Level Quality
- **Main conditions and standards** a piece of software must meet before deployment
- **Conditions for specific Product Backlog Item** acceptance (by customer, user, or other systems)
- **Tailored to individual items** — detail expected behavior and requirements of that feature/functionality
- **Focus**: Whether product increment fulfills specific requirements of Product Backlog Item
- **Primary responsibility**: Product Owner (can be delegated to Developers, often collaborative with stakeholders)
- **Scope**: Developed and tested for each user story individually (not product-wide)

### 3. DoD vs Acceptance Criteria — Key Differences
| Aspect | Definition of Done | Acceptance Criteria |
|--------|-------------------|---------------------|
| **Scope** | Product increment (overall) | Individual user story/PBI |
| **Focus** | Quality standards, usefulness, release readiness | Specific requirements fulfillment |
| **Responsibility** | Entire team / organization | Product Owner (+ stakeholders) |
| **Function** | Quality gate for increment | Quality gate for user story |
| **Consistency** | Uniform across all work | Tailored per item |
| **Level** | High-level checklist | Detailed feature expectations |

### 4. Google Code Review Standards
- **Open-source documentation**: [google/eng-practices](https://github.com/google/eng-practices) on GitHub
- **Primary purpose**: Ensure overall **code health improves over time**
- **Approval philosophy**: Favor approving CL (changelist) once it **definitely improves code health**, even if not perfect
- **Review focus areas**: Design, functionality, complexity, tests, naming
- **Decision hierarchy**: **Technical facts and data overrule opinions** and personal preferences; **style guide is absolute authority** on style matters
- **Scale**: One codebase shared by **25,000+ Googlers**, **40,000 commits daily**
- **Readability program**: Leads to more consistent baseline code quality vs similar-sized companies

### 5. Accelerate / DORA Metrics (Forsgren, Humble, Kim)
- **Book published 2018** — codifying 4 years of State of DevOps research (with Puppet)
- **Foundational finding**: **No tradeoff between speed and quality** — high performers excel at both
- **Software performance predicts company performance** (profit, market share, productivity)
- **Four key metrics** (DORA/Accelerate interchangeable):
  1. **Deployment Frequency**
  2. **Lead Time for Changes**
  3. **Time to Restore Service**
  4. **Change Failure Rate**
- **Balance**: First two lean toward Development (making changes), second two toward Operations (stability)
- **Research rigor**: Using State of DevOps data + rigorous statistical methods to measure software delivery performance and its drivers

### 6. Test-Driven Development (TDD) Impact
#### Quality Improvements:
- **40-90% reduction** in pre-release defect density vs similar non-TDD projects
- **76% of studies**: Significant increase in **internal software quality**
- **88% of studies**: Meaningful increase in **external software quality**
- **Code quality 2.6-4.2x better**
- **Block coverage 79-88%**

#### Productivity Trade-offs:
- **15-35% increase** in initial development time after TDD adoption
- **31% average overhead** in one project (developers took 31% more time developing items)
- **Small positive effect on quality**, little to no discernible effect on productivity (general finding)
- **Industrial vs academic**: Quality improvement and productivity drop both **much larger in industrial studies** than academic
- **2024 research** (September): Mixed-methods study (quantitative surveys + qualitative interviews) confirms TDD effectiveness in improving software quality

---

## Sources

### Definition of Done & Acceptance Criteria

1. **[How to Compare Acceptance Criteria vs. Definition of Done](https://www.techtarget.com/searchsoftwarequality/tip/How-to-compare-acceptance-criteria-vs-definition-of-done)** — TechTarget
   - DoD: agreed-upon set of items for completion
   - Acceptance criteria: main conditions for deployment

2. **[Definition of Done vs. Acceptance Criteria: A Complete Guide](https://nulab.com/learn/software-development/definition-of-done-vs-acceptance-criteria/)** — Nulab
   - DoD: high-level criteria for product increment
   - Acceptance criteria: specific PBI conditions

3. **[What is Agile Acceptance Criteria?](https://www.6sigma.us/six-sigma-in-focus/agile-acceptance-criteria/)** — SixSigma.us
   - Acceptance criteria definition
   - Quality gate function

4. **[What Is the Difference Between DoD and Acceptance Criteria?](https://www.scrum.org/resources/blog/what-difference-between-definition-done-and-acceptance-criteria)** — Scrum.org
   - Authoritative Scrum perspective
   - Key distinctions table

5. **[What is the Definition of Done (DoD) in Agile?](https://www.atlassian.com/agile/project-management/definition-of-done)** — Atlassian
   - DoD applies to all product increments
   - Defines overall product quality

6. **[Definition of Done vs. Acceptance Criteria: A Complete Guide](https://agilemania.com/definition-of-done-vs-acceptance-criteria)** — Agile Mania
   - DoD: comprehensive checklist (functionality, performance, security, compliance)
   - Quality gate comparison

7. **[The Agile Definition of Done: What Product Managers Need to Know](https://www.productplan.com/learn/agile-definition-of-done/)** — ProductPlan
   - DoD for product managers
   - Integration into workflows

8. **[Definition of Done. What it is, How it Works, Examples](https://learningloop.io/glossary/agile-definition-of-done)** — Learning Loop
   - Practical examples
   - Implementation guidance

9. **[DoD vs Acceptance Criteria: How to Ensure Software Quality and Improve Performance by 100 times](https://medium.com/beyond-agile-leadership/definition-of-done-vs-acceptance-criteria-how-to-ensure-software-quality-and-improve-performance-86aec2249e17)** — Eiki Takeuchi, Medium (Aug 2025)
   - Recent 2025 perspective
   - Performance improvement claims

10. **[The Definition of Done vs. Acceptance Criteria](https://www.forecast.app/learn/the-definition-of-done-vs-acceptance-criteria)** — Forecast
    - How they work together
    - DoD: uniform quality + completeness; AC: stakeholder-specific requirements

### Google Code Review Standards

11. **[The Standard of Code Review](https://google.github.io/eng-practices/review/reviewer/standard.html)** — Google eng-practices (Official)
    - Primary purpose: overall code health improves over time
    - Approval philosophy: favor approving when definitely improves

12. **[Introduction | eng-practices](https://google.github.io/eng-practices/review/)** — Google (Official)
    - Code review to maintain quality of code and products
    - Canonical documentation of processes/policies

13. **[GitHub - google/eng-practices](https://github.com/google/eng-practices)** — Google's Engineering Practices documentation
    - Open-source repository
    - Full documentation access

14. **[Google's Engineering Practices – Code Review Standards](https://www.codingblocks.net/podcast/googles-engineering-practices-code-review-standards/)** — Coding Blocks Podcast
    - Review focus: design, functionality, complexity, tests, naming
    - Technical facts/data overrule opinions

15. **[13 Code Review Standards Inspired by Google](https://betterprogramming.pub/13-code-review-standards-inspired-by-google-6b8f99f7fd67)** — Better Programming
    - Practical application of Google standards
    - Key principles extraction

16. **[Readability: Google's Temple to Engineering Excellence](https://www.moderndescartes.com/essays/readability/)** — Modern Descartes
    - Readability program details
    - 25,000+ Googlers sharing codebase
    - 40,000 commits daily
    - More consistent baseline quality

17. **[Google Guidance on Code Review](https://bssw.io/items/google-guidance-on-code-review)** — BSSW (Better Scientific Software)
    - Academic/scientific perspective on Google practices

18. **[How Google Does Code Reviews](https://www.freecodecamp.org/news/what-google-taught-me-about-code-reviews/)** — freeCodeCamp
    - Style guide = absolute authority on style
    - Favor technical facts over opinions

### Accelerate / DORA Metrics

19. **[Accelerate and DORA Metrics - Software Delivery Performance Measurement](https://openpracticelibrary.com/blog/accelerate-metrics-software-delivery-performance-measurement/)** — Open Practice Library
    - DORA/Accelerate metrics interchangeable
    - Four metrics: deployment frequency, lead time, time to restore, change failure rate

20. **[Accelerate: The Science of Lean Software and DevOps](https://books.google.com/books/about/Accelerate.html?id=Kax-DwAAQBAJ)** — Google Books
    - Book details (Forsgren, Humble, Kim)
    - Published 2018

21. **[Accelerate](https://itrevolution.com/product/accelerate/)** — IT Revolution
    - Official book page
    - Publisher information

22. **[Accelerate Book — Summary and Top Ideas](https://www.briansnotes.io/book/accelerate/)** — Brian's Notes
    - Four years of groundbreaking research
    - State of DevOps reports with Puppet
    - Rigorous statistical methods

23. **[Book Summary: Accelerate](https://andrewclark.co.uk/product-book-summaries/accelerate)** — Andrew Clark
    - No tradeoff between speed and quality
    - High performers excel at all measures
    - Software performance predicts company performance

24. **[What are Accelerate Metrics?](https://getdx.com/blog/accelerate-metrics/)** — DX
    - Metrics balance Development goals (making changes) vs Operations goals (stability)
    - Detailed metric breakdown

25. **[Accelerating DevOps With DORA Metrics](https://www.harness.io/blog/dora-metrics)** — Harness
    - DORA metrics application
    - DevOps acceleration strategies

### Test-Driven Development (TDD)

26. **[Evaluating the Impact of Test-Driven Development on Software Quality Enhancement](https://www.researchgate.net/publication/383694705_Evaluating_the_impact_of_Test-Driven_Development_on_Software_Quality_Enhancement)** — ResearchGate (September 2024)
    - Recent 2024 research
    - Mixed-methods approach (quantitative surveys + qualitative interviews)
    - TDD effectiveness in improving software quality

27. **[Realizing Quality Improvement Through Test Driven Development](https://dl.acm.org/doi/abs/10.1007/s10664-008-9062-z)** — ACM / Empirical Software Engineering (Vol 13, No 3)
    - Pre-release defect density decreased 40-90%
    - Comparison vs similar non-TDD projects

28. **[About the Return on Investment of Test-Driven Development](https://www.researchgate.net/publication/2849597_About_the_Return_on_Investment_of_Test-Driven_Development)** — ResearchGate
    - ROI analysis of TDD
    - Cost-benefit evaluation

29. **[Realizing Quality Improvement Through Test Driven Development](https://www.microsoft.com/en-us/research/wp-content/uploads/2009/10/Realizing-Quality-Improvement-Through-Test-Driven-Development-Results-and-Experiences-of-Four-Industrial-Teams-nagappan_tdd.pdf)** — Microsoft Research (PDF)
    - Case studies from four industrial teams
    - Results and experiences

30. **[The Effects of Test-Driven Development on External Quality and Productivity: A Meta-Analysis](https://www.researchgate.net/publication/260649027_The_Effects_of_Test-Driven_Development_on_External_Quality_and_Productivity_A_Meta-Analysis)** — ResearchGate
    - 76% of studies: significant increase in internal quality
    - 88% of studies: meaningful increase in external quality

31. **[Test-Driven Development: Is TDD Relevant in 2024?](https://www.scrumlaunch.com/blog/test-driven-development-in-2024)** — Scrum Launch (2024)
    - 2024 relevance assessment
    - Current industry perspective

32. **[The Effects of Test Driven Development on Internal Quality, External Quality and Productivity: A Systematic Review](https://www.sciencedirect.com/science/article/abs/pii/S0950584916300222)** — ScienceDirect
    - Systematic review methodology
    - Comprehensive quality assessment

33. **[Boost Code Quality with Test-Driven Development (TDD)](https://www.accelq.com/blog/tdd-test-driven-development/)** — accelQ
    - Code quality 2.6-4.2x better with TDD
    - Block coverage 79-88%

34. **[Effects of Test-Driven Development: A Comparative Analysis of Empirical Studies](https://www.researchgate.net/publication/256848134_Effects_of_Test-Driven_Development_A_Comparative_Analysis_of_Empirical_Studies)** — ResearchGate
    - 15-35% increase in initial development time
    - 31% average overhead in one project
    - Small positive effect on quality, little/no effect on productivity
    - Industrial studies: larger quality improvement AND larger productivity drop vs academic studies

---

## Statistics & Data Points

### Definition of Done
- **Comprehensive checklist**: Functionality, performance, security, compliance standards — [Source 6](https://agilemania.com/definition-of-done-vs-acceptance-criteria)
- **Applies to ALL product increments** (not just individual stories) — [Source 5](https://www.atlassian.com/agile/project-management/definition-of-done)
- **Created collaboratively**: Entire team, sometimes multiple teams or organization — [Source 4](https://www.scrum.org/resources/blog/what-difference-between-definition-done-and-acceptance-criteria)

### Google Code Review Scale
- **25,000+ Googlers** share one codebase — [Source 16](https://www.moderndescartes.com/essays/readability/)
- **40,000 commits daily** — [Source 16](https://www.moderndescartes.com/essays/readability/)
- **Readability program** → more consistent baseline quality — [Source 16](https://www.moderndescartes.com/essays/readability/)

### Accelerate / DORA
- **No tradeoff between speed and quality** — high performers excel at both — [Source 23](https://andrewclark.co.uk/product-book-summaries/accelerate)
- **Software performance predicts company performance** (profit, market share, productivity) — [Source 23](https://andrewclark.co.uk/product-book-summaries/accelerate)
- **4 years of research** — State of DevOps reports with Puppet — [Source 22](https://www.briansnotes.io/book/accelerate/)

### TDD Impact — Quality
- **40-90% reduction** in pre-release defect density — [Source 27](https://dl.acm.org/doi/abs/10.1007/s10664-008-9062-z)
- **76% of studies**: Significant **internal quality** increase — [Source 30](https://www.researchgate.net/publication/260649027_The_Effects_of_Test-Driven_Development_on_External_Quality_and_Productivity_A_Meta-Analysis)
- **88% of studies**: Meaningful **external quality** increase — [Source 30](https://www.researchgate.net/publication/260649027_The_Effects_of_Test-Driven_Development_on_External_Quality_and_Productivity_A_Meta-Analysis)
- **Code quality 2.6-4.2x better** — [Source 33](https://www.accelq.com/blog/tdd-test-driven-development/)
- **Block coverage 79-88%** — [Source 33](https://www.accelq.com/blog/tdd-test-driven-development/)

### TDD Impact — Productivity
- **15-35% increase** in initial development time — [Source 34](https://www.researchgate.net/publication/256848134_Effects_of_Test-Driven_Development_A_Comparative_Analysis_of_Empirical_Studies)
- **31% average overhead** (one project study) — [Source 34](https://www.researchgate.net/publication/256848134_Effects_of_Test-Driven_Development_A_Comparative_Analysis_of_Empirical_Studies)
- **Small positive effect on quality**, little/no effect on productivity (general) — [Source 34](https://www.researchgate.net/publication/256848134_Effects_of_Test-Driven_Development_A_Comparative_Analysis_of_Empirical_Studies)
- **Industrial vs academic**: Both quality improvement AND productivity drop **much larger** in industrial settings — [Source 34](https://www.researchgate.net/publication/256848134_Effects_of_Test-Driven_Development_A_Comparative_Analysis_of_Empirical_Studies)

---

## Case Examples

### Google's Code Review at Scale
- **Context**: 25,000+ Googlers, 40,000 commits/day, single codebase
- **Challenge**: Maintain quality and consistency at extreme scale
- **Approach**:
  - Code health improvement as primary goal (not perfection)
  - Technical facts/data overrule opinions
  - Style guide as absolute authority
  - Readability program for baseline consistency
- **Outcome**: More consistent baseline quality than similar-sized companies
- **Source**: [Modern Descartes](https://www.moderndescartes.com/essays/readability/), [Google eng-practices](https://google.github.io/eng-practices/review/)

### TDD in Four Industrial Teams (Microsoft Research)
- **Study**: Four industrial teams implementing TDD
- **Quality result**: 40-90% reduction in pre-release defect density
- **Productivity result**: 15-35% initial development time increase
- **Context**: Real-world industrial settings (not academic experiments)
- **Insight**: Quality gains significant; productivity impact moderate but measurable
- **Source**: [Microsoft Research PDF](https://www.microsoft.com/en-us/research/wp-content/uploads/2009/10/Realizing-Quality-Improvement-Through-Test-Driven-Development-Results-and-Experiences-of-Four-Industrial-Teams-nagappan_tdd.pdf)

### Accelerate Research: Speed ≠ Quality Tradeoff
- **Myth**: "Go fast OR maintain quality" (false dichotomy)
- **Finding**: High performers excel at **both** speed and quality (DORA metrics)
- **Broader impact**: Software delivery performance predicts **business performance**
- **Implication**: MQB/quality gates are not "slowing down" — they enable sustained speed
- **Source**: [Accelerate Summary](https://andrewclark.co.uk/product-book-summaries/accelerate)

### DoD vs AC in Practice
- **Example**: E-commerce checkout feature
  - **Acceptance Criteria** (feature-specific):
    - User can add/remove items from cart
    - Discount codes apply correctly
    - Payment processing succeeds
  - **Definition of Done** (product-wide):
    - Code reviewed and approved
    - Unit tests written and passing (>80% coverage)
    - Integration tests passing
    - Security scan clean
    - Performance: checkout completes <2 seconds
    - Documentation updated
    - Deployed to staging environment
- **Outcome**: AC ensures feature works; DoD ensures product-wide quality bar met
- **Source**: Synthesized from [Scrum.org](https://www.scrum.org/resources/blog/what-difference-between-definition-done-and-acceptance-criteria), [Atlassian](https://www.atlassian.com/agile/project-management/definition-of-done)

---

## Quotes for Book

> "The Definition of Done is an agreed-upon set of items that must be completed before a project or user story can be considered complete."
> — via [TechTarget](https://www.techtarget.com/searchsoftwarequality/tip/How-to-compare-acceptance-criteria-vs-definition-of-done)

> "The DoD is a set of high-level criteria for determining if a product increment is complete. It applies to all product increments and defines the overall quality of a product."
> — via [Nulab](https://nulab.com/learn/software-development/definition-of-done-vs-acceptance-criteria/)

> "The primary purpose of code review is to make sure that the overall code health of Google's code base is improving over time."
> — Google, via [eng-practices](https://google.github.io/eng-practices/review/reviewer/standard.html)

> "Reviewers should favor approving a CL once it is in a state where it definitely improves the overall code health of the system being worked on, even if the CL isn't perfect."
> — Google, via [eng-practices](https://google.github.io/eng-practices/review/reviewer/standard.html)

> "Technical facts and data overrule opinions and personal preferences, and on matters of style, the style guide is the absolute authority."
> — Google, via [Coding Blocks Podcast](https://www.codingblocks.net/podcast/googles-engineering-practices-code-review-standards/)

> "There is no tradeoff between speed and quality. High performers do better at all the measures. Additionally, software performance is a good predictor of company performance (profit, market share and productivity)."
> — Forsgren, Humble, Kim, via [Accelerate Summary](https://andrewclark.co.uk/product-book-summaries/accelerate)

> "Case studies indicate that pre-release defect density of four products decreased between 40% and 90% relative to similar projects that did not use TDD."
> — via [ACM / Empirical Software Engineering](https://dl.acm.org/doi/abs/10.1007/s10664-008-9062-z)

> "76% of studies identified a significant increase in internal software quality while 88% of studies identified a meaningful increase in external software quality."
> — via [ResearchGate Meta-Analysis](https://www.researchgate.net/publication/260649027_The_Effects_of_Test-Driven_Development_on_External_Quality_and_Productivity_A_Meta-Analysis)

---

## Anti-Patterns to Avoid

### 1. No Explicit DoD
- **Pattern**: Team has no written Definition of Done; "done" is subjective/negotiable
- **Evidence**: Inconsistent quality, rework, production bugs
- **Cost**: Technical debt accumulation, user dissatisfaction, support burden
- **Counter**: Collaboratively define DoD (entire team), enforce as quality gate

### 2. DoD as Ceremony
- **Pattern**: DoD exists on paper but is routinely bypassed under pressure ("ship it now, fix later")
- **Evidence**: MQB violations in production, "we'll tech-debt it" culture
- **Cost**: Erosion of standards, cascading quality issues (Ch 1: 87% budget on maintenance)
- **Counter**: Non-negotiable enforcement; leadership models adherence

### 3. Perfection Paralysis (Google Anti-Pattern)
- **Pattern**: Rejecting CLs that aren't "perfect" (vs "definitely improves code health")
- **Evidence**: Slow review cycles, frustrated developers, velocity drop
- **Cost**: Diminishing returns on quality, team morale damage
- **Counter**: Google's standard — "definitely improves" is sufficient (not "perfect")

### 4. TDD Abandonment Under Pressure
- **Pattern**: Writing tests first during calm periods, skipping tests when deadlines loom
- **Evidence**: Test coverage drops, defect rates spike, rework increases
- **Cost**: Loses 40-90% defect reduction benefit, defeats TDD ROI
- **Counter**: TDD as MQB requirement (non-negotiable, even under pressure)

### 5. Conflating AC and DoD
- **Pattern**: Treating acceptance criteria as sufficient for "done" (ignoring DoD)
- **Evidence**: Feature works in isolation but breaks product-wide standards (performance, security, accessibility)
- **Cost**: Integration failures, security vulnerabilities, accessibility violations
- **Counter**: AC = feature-specific gate; DoD = product-wide gate (both required)

### 6. Velocity Over Quality (DORA Myth)
- **Pattern**: Believing "speed OR quality" tradeoff exists; sacrificing quality for velocity
- **Evidence**: DORA research disproves this — high performers excel at both
- **Cost**: Accumulating tech debt slows future velocity (false economy)
- **Counter**: Quality gates enable sustained speed (Accelerate finding)

---

## Cross-References

### Related Chapters
- **Chapter 1 (Chaos)**: MQB as **chaos prevention** mechanism (quality gates vs bypasses)
- **Chapter 2 (HOTS)**: DoD/MQB as **leverage points** (rules, system structure)
- **Chapter 3 (Feature Factory)**: MQB prevents shipping outputs without quality/outcome validation
- **Chapter 5 (Purpose DNA)**: MQB includes **purpose alignment** checks (not just technical quality)
- **Chapter 7 (Experience DNA)**: MQB **operationalizes** Experience DNA thresholds (latency, reliability, accessibility)
- **Chapter 8 (Architecture DNA)**: MQB enforces **architectural fitness** (ADRs, dependency direction, observability)
- **Chapter 8 (Validation DNA)**: MQB includes **evidence requirements** (not assumptions)
- **Chapter 17 (Governance by Artifacts)**: DoD, AC, code review standards = **governance artifacts**

### Related Frameworks
- **Evolution Flow Cycle**: MQB gates at **Design → Build** and **Build → Validate** transitions
- **Builder's Hierarchy**: MQB ensures **feature quality** before escalating to capability/outcome levels
- **Cognitive Load Engineering** (Ch 14): Google's style guide, readability program reduce cognitive load

### Related DNAs
- **Purpose DNA**: MQB includes alignment checks (not just technical)
- **Experience DNA**: MQB thresholds (performance, accessibility, reliability)
- **Architecture DNA**: MQB enforces architectural standards (ADRs, patterns)
- **Validation DNA**: MQB requires evidence of validation (not "looks good to me")
- **Cultural DNA**: MQB adherence reflects cultural values (quality non-negotiable)

---

## MQB Components Framework (Synthesized)

Based on research, an effective MQB includes:

### 1. Functional Completeness
- Acceptance Criteria met (feature-specific)
- User story intent fulfilled
- Edge cases handled

### 2. Technical Quality
- Code review approved (Google standard: definitely improves code health)
- Tests written and passing (TDD: 40-90% defect reduction)
- Test coverage threshold met (e.g., 80% minimum)
- Static analysis clean (linters, security scanners)

### 3. Performance & Reliability
- Latency targets met (e.g., P95 <300ms for critical actions)
- Load testing passed (if applicable)
- Error handling robust (no silent failures)

### 4. Security & Compliance
- Security scan clean
- Compliance requirements met (GDPR, accessibility, industry-specific)
- Data handling standards followed

### 5. Documentation & Knowledge
- Code documented (inline comments for non-obvious logic)
- User-facing docs updated (if applicable)
- Architecture Decision Records updated (if design changed)

### 6. Deployment Readiness
- Deployed to staging/pre-production
- Integration tests passing
- Observability instrumented (logging, metrics, tracing)
- Rollback plan documented

### 7. Validation Evidence
- Assumption validated (not "we think it works")
- User testing conducted (if user-facing)
- Outcome metrics defined (how we'll know it succeeded)

---

## Open Questions

1. **MQB Calibration**: How do teams **calibrate** MQB over time? (Too strict = velocity drop; too loose = quality erosion)

2. **Context Dependency**: Does MQB vary by product stage? (Early-stage startup vs mature enterprise — likely yes, but how?)

3. **TDD ROI Threshold**: At what defect rate does TDD's 15-35% time investment **pay off**? (Break-even analysis)

4. **Google Model Transferability**: Can smaller orgs (e.g., 50-person teams) adopt Google's code review standards? (Scale considerations)

5. **DORA Causality**: Does high performance **cause** better business results, or do successful businesses **invest** in high performance? (Likely bidirectional)

6. **DoD Evolution**: How often should DoD be **revisited**? (Quarterly? Per major release? Continuous?)

7. **Automated Enforcement**: What % of MQB can be **automated** (CI/CD gates) vs requiring human judgment? (Maximize automation to reduce cognitive load)

---

## Next Research Steps

1. ✅ **Part I (Foundations) Research Complete**: Chaos, HOTS, Feature Factory, MQB
2. ⏭️ **Part II (8 DNAs)** — Begin detailed research:
   - Ch 5: Purpose DNA (Vision/mission, North Star, strategy deployment)
   - Ch 6: User DNA (JTBD, user research, personas)
   - Ch 7: Experience DNA (UX quality, Nielsen heuristics, accessibility)
   - Ch 8: Architecture/Data/Validation/Growth/Cultural DNAs
3. ⏭️ **Case studies**: Collect 3-5 examples of MQB transformations (chaos → quality discipline)
4. ⏭️ **Deeper TDD literature**: Kent Beck's "Test-Driven Development by Example"
5. ⏭️ **Expand quality frameworks**: Six Sigma, ISO 9001 (compare/contrast with MQB)

---

**TRACE:** `RESEARCH:CH04:MQB-STANDARDS:v1.0`
**Last Updated:** November 30, 2025
