# Chapter 8: Architecture DNA — Structural Stability & Evolution — Research

**Research Date:** November 30, 2025
**Researcher:** Mary (Business Analyst)
**Status:** In Progress

---

## Key Findings

### 1. Architecture Decision Records (ADRs) — Michael Nygard
- **Foundational work**: Michael Nygard's 2011 blog post **"Documenting Architecture Decisions"** popularized ADRs
- **First incarnation**: Nygard's template considered "the first incarnation of the term 'ADR'"
- **Purpose**: Capture **single architectural decision and its rationale** — help teams understand reasons for decisions, trade-offs, consequences
- **Template structure** (Nygard's format):
  1. **Title**: Descriptive (usually in file/document name)
  2. **Date**
  3. **Status**: proposed, accepted, rejected, deprecated, superseded
  4. **Context**: Motivation/problem + context needed to understand
  5. **Decision**: Details and specifics of proposed change
  6. **Consequences**: Positive/negative effects on other architecture parts
- **Key resource**: joelparkerhenderson/architecture-decision-record GitHub repo (templates and examples)

### 2. Building Evolutionary Architectures — Ford, Parsons, Kua
- **Authors**: Neal Ford, Rebecca Parsons, Patrick Kua (ThoughtWorks)
- **Core definition**: "An evolutionary architecture supports **guided, incremental change** across multiple dimensions"
- **Foundation**: Incremental developments in core engineering practices created foundations for rethinking architecture evolution over time
- **Fitness Functions** (core concept):
  - **Definition**: "Objective integrity assessment of some architectural characteristic(s)"
  - **Borrowed from**: Evolutionary computing / genetic algorithm design (defines success)
  - **Implementation**: Wide variety — tests, metrics, monitoring, logging
  - **Purpose**: Protect one or more architectural dimensions
- **Three primary concerns**:
  1. **Fitness functions**
  2. **Incremental change**
  3. **Appropriate coupling**
- **Framework**: Identify important architectural dimensions → define fitness functions to protect them → use modern engineering practices (deployment pipelines) to automatically verify characteristics don't degrade

### 3. Conway's Law & Team Topologies
- **Conway's Law**: "Organizations which design systems are constrained to produce designs which are copies of the communication structures of these organizations"
- **Inverse Conway Maneuver**: Deliberately design organizational structure to mirror desired system architecture
- **Team Topologies** (Skelton & Pais, 2019): Book-length treatment of Inverse Conway Maneuver
- **Key observation**: "Not all communication and collaboration is good"
- **Application**: Understanding Conway's Law is cornerstone for good team design

---

## Sources

### Architecture Decision Records (ADRs)

1. **[Architectural Decision Records (ADRs)](https://adr.github.io/)** — Official ADR Resource
   - Official community resource
   - Templates and best practices

2. **[ADR Template by Michael Nygard](https://github.com/joelparkerhenderson/architecture-decision-record/blob/main/locales/en/templates/decision-record-template-by-michael-nygard/index.md)** — GitHub
   - Original Nygard template
   - Markdown format

3. **[Architecture Decision Record Examples](https://github.com/joelparkerhenderson/architecture-decision-record)** — GitHub (joelparkerhenderson)
   - Examples for software planning
   - IT leadership and template documentation
   - Key resource repository

4. **[Architecture Decisions | arc42 Documentation](https://docs.arc42.org/section-9/)**
   - arc42 framework integration
   - Architecture documentation standards

5. **[ADR Template by Michael Nygard](https://github.com/jamesmh/architecture_decision_record/blob/master/adr_template_by_michael_nygard.md)** — GitHub (jamesmh)
   - Alternative repository
   - Same Nygard template

6. **[A Practical Overview on ADR](https://ctaverna.github.io/adr/)**
   - Practical implementation guide
   - Real-world application

7. **[Architectural Decision Records (ADR)](https://openpracticelibrary.com/practice/architectural-decision-records-adr/)** — Open Practice Library
   - 2011 blog post by Michael Nygard popularized concept
   - "First incarnation of the term 'ADR'"

8. **[Architecture Decision Records (ADRs)](https://icepanel.medium.com/architecture-decision-records-adrs-5c66888d8723)** — IcePanel, Medium
   - Capture single architectural decision and rationale
   - Help teams understand reasons, trade-offs, consequences

9. **[Architecture Decision Records Example](https://www.lasssim.com/architecture-decision-records-example/)**
   - Template structure: Title, Date, Status, Context, Decision, Consequences

### Building Evolutionary Architectures

10. **[Building Evolutionary Architectures (Google Books)](https://books.google.com/books/about/Building_Evolutionary_Architectures.html?id=BmudEAAAQBAJ)**
    - Full book details
    - Ford, Parsons, Kua, Sadalage

11. **[Building Evolutionary Architectures](https://nealford.com/books/buildingevolutionaryarchitectures.html)** — Neal Ford Official
    - Author's official book page
    - Resources and links

12. **[Fitness Functions](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/ch02.html)** — O'Reilly (Chapter 2)
    - Fitness functions chapter
    - Detailed explanation

13. **[Building Evolutionary Architectures [Book]](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/)**
    - Full O'Reilly book
    - Comprehensive resource

14. **[Building Evolutionary Architectures (PDF)](https://www.thoughtworks.com/content/dam/thoughtworks/documents/books/bk_building_evolutionary_architectures_en.pdf)** — ThoughtWorks
    - ThoughtWorks official PDF
    - Free resource

15. **[Building Evolutionary Architectures](https://evolutionaryarchitecture.com/)** — Official Website
    - Evolutionary architecture supports guided, incremental change across multiple dimensions
    - Incremental developments created foundations for rethinking architecture evolution

16. **[Building Evolutionary Architectures (Google Books - 2017)](https://books.google.com/books/about/Building_Evolutionary_Architectures.html?id=pYI2DwAAQBAJ)**
    - Original 2017 edition
    - Support Constant Change subtitle

17. **[Fitness Functions Definition](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/ch02.html)**
    - "Objective integrity assessment of some architectural characteristic(s)"
    - Borrowed from evolutionary computing
    - Wide variety: tests, metrics, monitoring, logging

18. **[Three Primary Concerns](https://evolutionaryarchitecture.com/)**
    - Fitness functions, incremental change, appropriate coupling
    - ThoughtWorks specialists examine each separately, then combine

### Conway's Law & Team Topologies

19. **[Team Topologies](https://jacobian.org/2021/jul/5/book-review-team-topologies/)** — Jacob Kaplan-Moss
    - Book review perspective
    - Practical applications

20. **[Book Review: "Team Topologies"](https://embeddeduse.com/2022/04/23/book-review-team-topologies-by-matthew-skelton-and-manuel-pais/)** — Embedded Use
    - Skelton and Pais 2019 book
    - Comprehensive review

21. **[Team Topologies - Organizing for Fast Flow](https://teamtopologies.com/)** — Official Website
    - Leading approach to organizing teams
    - Fast flow of value and business agility

22. **[Team Topologies](https://martinfowler.com/bliki/TeamTopologies.html)** — Martin Fowler
    - Conway's Law: "Organizations constrained to produce designs copying their communication structures"
    - Understanding Conway's Law = cornerstone for good team design

23. **[Team Topologies: Key Insights](https://andrewmatveychuk.com/notes-on-team-topologies-by-matthew-skelton-and-manuel-pais-book-review)** — Andrew Matveychuk
    - Key observation: "Not all communication and collaboration is good"

24. **[Book Notes: Team Topologies](https://danlebrero.com/2021/01/20/team-topologies-summary/)**
    - Published September 2019 by IT Revolution Press
    - Team Topologies == 4 team types + 3 interactions + Conway's law + Cognitive Load + Sensing + evolution

25. **[Team Topologies Book Review](https://maa1.medium.com/team-topologies-book-review-ecaad8d9e165)** — MAA1, Medium
    - Inverse Conway Maneuver: deliberately design org structure to mirror desired system
    - Book-length treatment of this principle

---

## Statistics & Data Points

### ADR Adoption
- **2011**: Michael Nygard blog post popularized ADRs — [Source 7](https://openpracticelibrary.com/practice/architectural-decision-records-adr/)
- **Template elements**: 6 core sections (Title, Date, Status, Context, Decision, Consequences) — [Source 9](https://www.lasssim.com/architecture-decision-records-example/)

### Evolutionary Architecture
- **Three primary concerns**: Fitness functions + Incremental change + Appropriate coupling — [Source 18](https://evolutionaryarchitecture.com/)

### Team Topologies
- **Published**: September 2019, IT Revolution Press — [Source 24](https://danlebrero.com/2021/01/20/team-topologies-summary/)

---

## Quotes for Book

> "Organizations which design systems are constrained to produce designs which are copies of the communication structures of these organizations."
> — Conway's Law, via [Martin Fowler](https://martinfowler.com/bliki/TeamTopologies.html)

> "An evolutionary architecture supports guided, incremental change across multiple dimensions."
> — Ford, Parsons, Kua, via [Evolutionary Architecture](https://evolutionaryarchitecture.com/)

> "An architectural fitness function provides an objective integrity assessment of some architectural characteristic(s)."
> — Ford, Parsons, Kua, via [O'Reilly](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/ch02.html)

> "Understanding Conway's law is the cornerstone for good team design."
> — Skelton & Pais, via [Martin Fowler](https://martinfowler.com/bliki/TeamTopologies.html)

> "One key observation the book makes is that: Not all communication and collaboration is good."
> — Team Topologies, via [Andrew Matveychuk](https://andrewmatveychuk.com/notes-on-team-topologies-by-matthew-skelton-and-manuel-pais-book-review)

> "Michael Nygard's 2011 blog post 'Documenting Architecture Decisions' popularized the concept of ADRs."
> — via [Open Practice Library](https://openpracticelibrary.com/practice/architectural-decision-records-adr/)

---

## Cross-References

### Related Chapters
- **Chapter 4 (MQB)**: ADRs as **quality gate** (architecture decisions documented)
- **Chapter 5 (Purpose DNA)**: Architecture **serves Purpose** (strategic needs → architectural constraints)
- **Chapter 7 (Experience DNA)**: Architecture **enables experience** (latency, reliability, scalability)
- **Chapter 12 (Cultural DNA)**: Conway's Law — **culture shapes architecture**
- **Chapter 14 (Systems Lens)**: Deep dive into modular architecture patterns
- **Chapter 21 (Governance by Artifacts)**: ADRs as **governance mechanism**

### Related Frameworks
- **Evolution Flow**: Architecture decisions in **Design phase** (ADRs created)
- **Fitness Functions**: Automated **MQB enforcement** (architecture quality gates)
- **Inverse Conway Maneuver**: Org design → system design alignment

### Related DNAs
- **Purpose DNA**: Architecture decisions **traceable to Purpose**
- **Experience DNA**: Architecture **supports UX thresholds**
- **Data DNA**: Data architecture **part of overall architecture**
- **Cultural DNA**: Team structure **influences architecture** (Conway's Law)

---

## Next Research Steps

1. ✅ **Architecture DNA research complete** (ADRs, Evolutionary Architectures, Conway's Law)
2. ⏭️ **Chapter 9: Data DNA** — Kleppmann, data-intensive applications
3. ⏭️ **Chapter 10: Validation DNA** — Experimentation, A/B testing (Kohavi)
4. ⏭️ **Chapter 11: Growth DNA** — Growth loops, AARRR metrics
5. ⏭️ **Chapter 12: Cultural DNA** — Netflix, Spotify, Team Topologies (full treatment)

---

**TRACE:** `RESEARCH:CH08:ARCHITECTURE-DNA:v1.0`
**Last Updated:** November 30, 2025
