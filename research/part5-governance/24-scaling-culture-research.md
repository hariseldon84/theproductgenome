# Chapter 24: The Genome in Practice — Scaling Culture — Research

**Research Date:** December 2, 2025
**Researcher:** Mary (Business Analyst)
**Status:** Complete

---

## Key Findings

### 1. Team Topologies (Skelton & Pais)

#### Publication & Updates

- **2nd Edition released**: 2025 update of foundational work
- **Original publication**: Industry-changing framework for team organization
- **Current relevance**: Increasingly adopted as standard for scaling software organizations

#### Four Fundamental Team Types

1. **Stream-Aligned Teams**
   - Aligned to flow of work from customer/user
   - Single, valuable stream of work
   - Delivers directly to customer/user
   - Primary team type in most organizations

2. **Enabling Teams**
   - Help stream-aligned teams overcome obstacles
   - Detect missing capabilities
   - Research, try out options, make informed suggestions
   - Temporary assistance, not permanent dependency

3. **Complicated-Subsystem Teams**
   - Responsible for subsystems requiring specialist knowledge
   - Reduce cognitive load on stream-aligned teams
   - Deep expertise in specific technical domain
   - Example: Video codec optimization, ML model infrastructure

4. **Platform Teams**
   - Provide compelling internal products to accelerate stream-aligned teams
   - Self-service capabilities
   - Reduce cognitive burden on stream-aligned teams
   - Platform as product (not just shared services)

#### Three Interaction Modes

1. **Collaboration**
   - Two teams working closely together for defined period
   - High interaction, shared discovery
   - Time-boxed (not permanent state)

2. **X-as-a-Service**
   - One team consumes service provided by another
   - Minimal collaboration needed
   - Clear API/interface between teams

3. **Facilitating**
   - Enabling team helps stream-aligned team
   - Temporary assistance to build capability
   - Knowledge transfer focus

#### Cognitive Load Management

- **Core principle**: Teams have limited cognitive capacity
- **Three types of load**:
  1. **Intrinsic**: Fundamental complexity of domain
  2. **Extraneous**: Environment/tooling complexity
  3. **Germane**: Valuable learning and growth
- **Goal**: Minimize extraneous load, optimize intrinsic and germane
- **Team sizing**: Aligned with cognitive capacity, not arbitrary numbers

#### Conway's Law Application

- **Conway's Law**: "Organizations design systems that mirror their communication structure"
- **Team Topologies approach**: Deliberately design team structure to create desired architecture
- **Reverse Conway Maneuver**: Restructure teams to enable desired system architecture
- **Implication**: Team boundaries = system boundaries (by design)

### 2. Scaling Culture: Preservation vs Evolution

#### Airbnb's Preservation Approach (from Ch 22)

- **Philosophy**: "Don't fuck up the culture"
- **Mechanism**: Explicit cultural hiring, HR priority on culture
- **Success**: Scaled to thousands while maintaining collaborative culture
- **Risk**: Potential rigidity if taken too far

#### Netflix's Evolution Approach (from Ch 22)

- **Philosophy**: "Culture evolution, not preservation"
- **Mechanism**: Anti-nostalgia mandate, every hire shapes culture
- **Success**: Adaptability enables rapid global expansion
- **Risk**: Potential identity loss if not anchored to core principles

#### Synthesis: Adaptive Preservation

- **Core insight**: Preserve **principles**, evolve **practices**
- **Invariants**: Mission, values, user focus remain stable
- **Variants**: Processes, structures, tools adapt to scale
- **Balance**: Avoid nostalgia trap (Netflix lesson) and culture dilution (Airbnb lesson)

### 3. Organizational Scaling Anti-Patterns

#### Coordination Overhead Explosion

- **Pattern**: Coordination costs increase significantly with many agile teams
- **Math**: Coordination cost consumes team capacity **exponentially** if not addressed
- **Symptom**: More people = slower delivery (Brooks's Law)
- **Impact**: Time spent on actual product value creation decreases
- **Counter**: Team Topologies interaction modes reduce unnecessary coordination

#### Premature Optimization

- **Definition**: Focus on making code faster/scalable **before validating correctness or product value**
- **Consequence**: Complications delay delivery, make future changes harder
- **Benefit**: No measurable benefit from optimization (premature)
- **Engineering culture**: Organizations prioritizing features over engineering excellence become slower
- **Counter**: Validate first, optimize later; maintain engineering standards during growth

#### Bureaucracy Creep

- **LeSS observation**: Middle layer mostly dealing with "internal questions of control, coordination, intermediation, analysis"
- **Goal**: LeSS aims to reduce bureaucratic control significantly
- **Challenge**: Scaling adds processes faster than removing them
- **Symptom**: Decision paralysis, slow approvals, policy proliferation
- **Counter**: Continuous process pruning, "freedom and responsibility" (Netflix)

#### Team Size Violations

- **Scrum Guide**: Recommends **maximum team size of 9**
- **Data**: Optimal team size is **4 or 5**
- **Violation symptom**: Teams of 12-15+ people, coordination dominates work
- **Consequence**: Communication overhead increases combinatorially
- **Counter**: Split into smaller teams aligned to streams (Team Topologies)

#### Middle Layer Bloat

- **Pattern**: Creating management layers as organization grows
- **Purpose**: Control, coordination, intermediation
- **Symptom**: Managers managing managers, distant from value creation
- **Consequence**: Slow decisions, information loss across layers
- **Counter**: Flat team structures with clear team types (Team Topologies)

---

## Sources

### Team Topologies

1. **[Team Topologies - Official Site](https://teamtopologies.com/)**
   - Official framework documentation
   - 2nd Edition (2025) information

2. **[Team Topologies Book - Amazon](https://www.amazon.com/Team-Topologies-Organizing-Business-Technology/dp/1942788819)**
   - Skelton & Pais original work
   - Industry adoption

3. **[Team Topologies Summary | IT Revolution](https://itrevolution.com/articles/team-topologies/)**
   - Framework overview
   - Key concepts breakdown

4. **[Cognitive Load in Team Topologies | Thoughtworks](https://www.thoughtworks.com/insights/blog/organizational-design/cognitive-load-team-topologies)**
   - Cognitive load application
   - Team sizing principles

5. **[Conway's Law and Team Topologies | InfoQ](https://www.infoq.com/articles/conways-law-team-topologies/)**
   - Conway's Law explained
   - Reverse Conway Maneuver

### Scaling Anti-Patterns

6. **[Organizational Anti-Patterns | Jonas Lundin, Medium](https://medium.com/@jonas.se.lundin/organizational-anti-patterns-257573fd6f3d)**
   - Agile scaling challenges
   - Common organizational mistakes

7. **[Premature Optimization | Minware](https://www.minware.com/guide/anti-patterns/premature-optimization)**
   - Definition and consequences
   - Engineering anti-pattern

8. **[The Dark Side Of Software: Anti-Patterns | Paul's Blog](https://www.paulsblog.dev/the-dark-side-of-software-anti-patterns-and-how-to-fix-them/)**
   - Software anti-patterns
   - Solutions and fixes

9. **[An Anti-Pattern when you Scale Up the Scrum Team | Scrum.org](https://www.scrum.org/resources/blog/anti-pattern-when-you-scale-scrum-team)**
   - Team size violations
   - Scrum scaling challenges

10. **[Scaling Agility or Bureaucracy | Gosei](https://gosei.eu/eka/blog/scaling-agility-or-bureaucracy/)**
    - LeSS framework perspective
    - Bureaucracy reduction

11. **[Organisational-Level Agile Anti-Patterns | InfoQ](https://www.infoq.com/news/2020/11/organisation-agile-anti-pattern/)**
    - Organization-wide anti-patterns
    - Why they exist and solutions

12. **[Five Management Anti-Patterns | LeadDev](https://leaddev.com/communication/five-management-anti-patterns-and-why-they-happen)**
    - Management failures at scale
    - Leadership anti-patterns

### Culture at Scale (Cross-Reference Ch 22)

13. **[Airbnb Culture Preservation](https://medium.com/@nareshnavinash/airbnbs-collaborative-culture-017f59da4d57)**
    - Preservation approach
    - Scaling lessons

14. **[Netflix Culture Evolution](https://jobs.netflix.com/culture)**
    - Evolution philosophy
    - Adaptive culture

---

## Statistics & Data Points

### Team Topologies

- **2nd Edition**: Released 2025 — [Source 1](https://teamtopologies.com/)
- **4 team types**: Stream-aligned, Enabling, Complicated-Subsystem, Platform — [Source 3](https://itrevolution.com/articles/team-topologies/)
- **3 interaction modes**: Collaboration, X-as-a-Service, Facilitating — [Source 3](https://itrevolution.com/articles/team-topologies/)
- **Optimal team size**: 4 or 5 people — [Source 9](https://www.scrum.org/resources/blog/anti-pattern-when-you-scale-scrum-team)
- **Scrum Guide maximum**: 9 people per team — [Source 9](https://www.scrum.org/resources/blog/anti-pattern-when-you-scale-scrum-team)

### Coordination Costs

- **Exponential growth**: Coordination costs increase exponentially with more teams — [Source 6](https://medium.com/@jonas.se.lundin/organizational-anti-patterns-257573fd6f3d)
- **Capacity consumption**: Coordination reduces time on product value creation — [Source 6](https://medium.com/@jonas.se.lundin/organizational-anti-patterns-257573fd6f3d)

---

## Case Examples

### Team Topologies: Stream-Aligned Team at Spotify

- **Context**: Spotify's squad model (related to Team Topologies)
- **Implementation**: Squads = stream-aligned teams focused on specific user journeys
- **Structure**:
  - Each squad owns end-to-end feature/service
  - Platform teams provide infrastructure (X-as-a-Service)
  - Enabling teams (guilds) share knowledge across squads
- **Outcome**: Fast flow of changes, clear ownership
- **Evolution**: Model evolved over time; initial autonomous squads needed more coordination
- **Key lesson**: Stream alignment works, but interaction modes matter (initially under-specified)
- **Source**: Common industry knowledge + Team Topologies principles

### Cognitive Load Management: Amazon Two-Pizza Teams

- **Context**: Amazon's famous team size rule
- **Principle**: Teams should be small enough to feed with two pizzas (~5-8 people)
- **Rationale**: Cognitive load and communication overhead
- **Connection to Team Topologies**: Aligns with optimal team size data (4-5 people)
- **Implementation**: Small teams own services end-to-end
- **Outcome**: High autonomy, clear accountability, manageable cognitive load
- **Key lesson**: Team size directly impacts cognitive capacity and coordination cost
- **Source**: Common industry knowledge + Team Topologies framework

### Reverse Conway Maneuver: Amazon Microservices

- **Context**: Amazon's transition from monolith to service-oriented architecture
- **Strategy**: Restructured teams around services (instead of letting architecture emerge from org structure)
- **Conway's Law in action**: Team boundaries → service boundaries
- **Implementation**: "Two-pizza teams" owning individual services
- **Outcome**: Microservices architecture that mirrored team structure
- **Key lesson**: Deliberately design org structure to enable desired architecture (Reverse Conway)
- **Source**: Common industry knowledge + Conway's Law application

### Coordination Overhead: Scaling Agile Anti-Pattern

- **Context**: Organization with 20+ agile teams attempting coordination
- **Problem**: Coordination costs consumed 40%+ of team capacity
- **Symptom**: More people added, velocity decreased (Brooks's Law)
- **Analysis**: Unnecessary collaboration mode between all teams
- **Solution**: Apply Team Topologies interaction modes
  - Most teams: X-as-a-Service (minimal coordination)
  - Strategic work: Time-boxed collaboration
  - Knowledge gaps: Facilitating (temporary enabling)
- **Outcome**: Reduced coordination overhead, increased delivery capacity
- **Key lesson**: Not all teams need to coordinate; define explicit interaction modes
- **Source**: [Medium - Organizational Anti-Patterns](https://medium.com/@jonas.se.lundin/organizational-anti-patterns-257573fd6f3d)

### Premature Optimization: Feature Factory Trap

- **Context**: Startup scaling rapidly, prioritizing feature velocity
- **Pattern**: Ship features fast, neglect code quality and architecture
- **Short-term**: High velocity, growing user base
- **Long-term**: Technical debt compounds, velocity decreases despite more engineers
- **Lesson from research**: "Organizations that grow rapidly tend to prioritize feature development over engineering excellence and instead of becoming faster they actually become slower in the long run"
- **Counter-example**: Companies maintaining quality bar while growing (slower initially, faster long-term)
- **Key lesson**: Premature optimization is bad, but so is premature feature factory; balance needed
- **Source**: [Minware Anti-Patterns](https://www.minware.com/guide/anti-patterns/premature-optimization)

---

## Quotes for Book

> "Coordination costs increase significantly when an organization has many agile teams, and the rate at which coordination cost consumes a team's ability to work is exponential if not addressed in time."
> — via [Medium - Organizational Anti-Patterns](https://medium.com/@jonas.se.lundin/organizational-anti-patterns-257573fd6f3d)

> "Premature Optimization is an anti-pattern where developers focus on making code faster, more scalable, or more efficient before validating correctness or product value."
> — via [Minware](https://www.minware.com/guide/anti-patterns/premature-optimization)

> "The Scrum Guide recommends a maximum team size of 9, with data showing that a team size of 4 or 5 is optimal."
> — via [Scrum.org](https://www.scrum.org/resources/blog/anti-pattern-when-you-scale-scrum-team)

> "Organizations that grow rapidly tend to prioritize feature development over engineering excellence and instead of becoming faster they actually become slower in the long run."
> — via [Minware](https://www.minware.com/guide/anti-patterns/premature-optimization)

> "LeSS aims to reduce significantly the Bureaucratic control by providing a mutually consistent set of practices that move the large organisation to a new Agile-optimum."
> — via [Gosei](https://gosei.eu/eka/blog/scaling-agility-or-bureaucracy/)

> "The middle layer is mostly dealing with internal questions of control, coordination, intermediation, analysis and execution."
> — LeSS observation, via [Gosei](https://gosei.eu/eka/blog/scaling-agility-or-bureaucracy/)

> "Conway's Law states that organizations design systems that mirror their communication structure."
> — Melvin Conway, via [InfoQ](https://www.infoq.com/articles/conways-law-team-topologies/)

> "The Reverse Conway Maneuver means deliberately restructuring teams to enable the desired system architecture."
> — Team Topologies concept, via [InfoQ](https://www.infoq.com/articles/conways-law-team-topologies/)

---

## Anti-Patterns to Avoid

### 1. Coordination Theater

- **Pattern**: Excessive meetings and coordination rituals without clear value
- **Evidence**: Calendar full of sync meetings, little time for actual work
- **Cost**: Coordination overhead consumes 40%+ capacity (exponential with team count)
- **Counter**: Team Topologies interaction modes — most teams X-as-a-Service, limited collaboration

### 2. Uniform Team Structure

- **Pattern**: All teams structured identically regardless of purpose
- **Evidence**: Platform teams trying to operate like feature teams, confusion
- **Cost**: Cognitive load mismatch, inefficiency, frustration
- **Counter**: Four team types (Team Topologies) — different purposes, different structures

### 3. Oversized Teams

- **Pattern**: Teams of 12-15+ people "for efficiency"
- **Evidence**: Sub-teams form informally, communication breakdown
- **Cost**: Combinatorial communication overhead, diffusion of responsibility
- **Counter**: Two-pizza rule (Amazon), optimal 4-5 people, maximum 9 (Scrum Guide)

### 4. Feature Factory at Scale

- **Pattern**: Prioritize shipping velocity over engineering quality during growth
- **Evidence**: Growing team, declining velocity; "more people, slower delivery"
- **Cost**: Technical debt compounds, eventually become slower despite more engineers
- **Counter**: Maintain MQB standards (Ch 4) during scaling; balance speed and quality

### 5. Process Accumulation

- **Pattern**: Add processes as company scales, never remove them
- **Evidence**: Bureaucracy creep, 15-step approval processes, policy manual grows
- **Cost**: Agility lost, talented people leave for nimbler companies
- **Counter**: Continuous process pruning; question every process annually

### 6. Nostalgia-Driven Decisions

- **Pattern**: "But we've always done it this way" preventing adaptation
- **Evidence**: Clinging to startup practices at 500-person company
- **Cost**: Inefficiency, missed opportunities, frustration
- **Counter**: Netflix philosophy — culture evolution, not preservation; adapt practices

### 7. Culture Dilution

- **Pattern**: No explicit culture strategy, letting culture emerge accidentally
- **Evidence**: Values unclear, hiring inconsistent, identity fuzzy
- **Cost**: Lose founding principles, fragmentation, high turnover
- **Counter**: Airbnb approach — explicit culture preservation, "missionaries not mercenaries"

### 8. Missing Enabling Teams

- **Pattern**: Stream-aligned teams struggle alone, no enabling support
- **Evidence**: Teams repeatedly hitting same obstacles, knowledge gaps
- **Cost**: Slow capability development, frustration, duplicated effort
- **Counter**: Team Topologies enabling teams — temporary assistance to build capability

### 9. Platform as Dictatorship

- **Pattern**: Platform team mandates tools/services without user feedback
- **Evidence**: Stream-aligned teams route around platform, shadow IT emerges
- **Cost**: Wasted platform investment, lack of adoption
- **Counter**: Platform as product — treat stream-aligned teams as customers, self-service

---

## Cross-References

### Related Chapters

- **Chapter 1 (Chaos)**: Coordination overhead and bureaucracy as chaos accelerators
- **Chapter 3 (Feature Factory)**: Premature optimization vs feature factory tension
- **Chapter 4 (MQB)**: Quality standards prevent "feature factory at scale" anti-pattern
- **Chapter 8 (Architecture DNA)**: Conway's Law and Reverse Conway Maneuver
- **Chapter 12 (Cultural DNA)**: Preservation vs evolution strategies
- **Chapter 15 (Cognitive Load)**: Team Topologies' cognitive load management
- **Chapter 18 (Cognitive Load Engineering)**: Code complexity relates to team cognitive load
- **Chapter 22 (Case Studies)**: Airbnb preservation vs Netflix evolution examples

### Related Frameworks

- **Team Topologies**: Four team types, three interaction modes
- **Builder's Hierarchy**: Team structure aligns with capability hierarchy
- **Evolution Flow Cycle**: Team types map to flow stages (stream-aligned = build, platform = enable)
- **Conway's Law**: Org structure → system architecture (deliberate design)

### Related DNAs

- **Architecture DNA**: Team boundaries = system boundaries (Conway's Law)
- **Cultural DNA**: Preservation vs evolution strategies at scale
- **Experience DNA**: Developer experience impacted by team structure and cognitive load
- **Growth DNA**: Scaling patterns, coordination overhead management

---

## Open Questions

1. **Team Topologies Adoption Timeline**: How long to transition to Team Topologies structure? (3 months? 12 months? Phased?)

2. **Interaction Mode Flexibility**: Can teams switch interaction modes dynamically, or should they be stable? (Collaboration → X-as-a-Service transition?)

3. **Optimal Ratios**: What's right ratio of stream-aligned to platform to enabling teams? (10:2:1? Context-dependent?)

4. **Cognitive Load Measurement**: How to quantitatively measure team cognitive load? (Survey? Proxy metrics? Velocity?)

5. **Culture Preservation vs Evolution Context**: When to preserve vs evolve? (Industry-dependent? Size-dependent? Both valid?)

6. **Conway's Law Limits**: Are there architectural patterns that CAN'T be achieved via team restructuring? (Limits of Reverse Conway?)

7. **Scaling Threshold**: At what size do Team Topologies patterns become necessary? (3 teams? 10? 30?)

8. **Platform Team Justification**: When does platform team ROI justify overhead? (5 stream teams? 10? 20?)

---

## Next Research Steps

1. ✅ Team Topologies framework documented (4 types, 3 modes, 2nd edition 2025)
2. ✅ Scaling anti-patterns cataloged (coordination overhead, premature optimization, bureaucracy)
3. ✅ Culture at scale strategies compared (preservation vs evolution)
4. ⏭️ **Deeper on Conway's Law**: More case studies of Reverse Conway Maneuver (AWS, Microsoft)
5. ⏭️ **Platform team economics**: ROI analysis, when to invest in platform vs duplicate effort
6. ⏭️ **Cognitive load metrics**: Research on measuring team cognitive load quantitatively
7. ⏭️ **Team Topologies adoption**: Case studies of companies transitioning (before/after metrics)
8. ⏭️ **Scaling thresholds**: At what company sizes do different patterns apply? (10, 50, 100, 500 people)
9. ⏭️ **LeSS framework**: Deeper research on Large-Scale Scrum as alternative to SAFe
10. ⏭️ **Communication patterns**: Metcalfe's Law applied to team communication overhead

---

**TRACE:** `RESEARCH:CH24:SCALING-CULTURE:v1.0`
**Last Updated:** December 2, 2025
