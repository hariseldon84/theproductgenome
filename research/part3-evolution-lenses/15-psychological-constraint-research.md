# Chapter 15: Psychological & Constraint Lenses — Research

**Research Date:** December 2, 2025
**Researcher:** Mary (Business Analyst)
**Status:** Complete

---

## Key Findings

### 1. Cognitive Load Theory (John Sweller)

- **Cognitive load** refers to the mental effort users spend while reading software artifacts
- **Three types of cognitive load**:
  - **Intrinsic**: Inherent difficulty of the material itself
  - **Extraneous**: Cognitive load caused by poor design/presentation
  - **Germane**: Productive cognitive load that contributes to learning/schema construction
- **Working memory capacity** is limited — learning is hampered when capacity is exceeded
- **Complexity in software** manifests as change amplification (changes becoming harder) and cognitive load (juggling more things mentally)
- **Two primary sources of complexity**:
  - **Dependencies**: When code cannot be understood/changed in isolation
  - **Obscurity**: When vital information is not apparent
- **43% of studies** analyzed cognitive load using combination of sensors
- **83% of studies** analyzed cognitive load during programming tasks specifically

### 2. Mental Models (Don Norman)

- **Mental models** are "what people really have in their heads and what guides their use of things"
- **Conceptual models** are devised as tools for understanding or teaching systems
- **Three aspects to mental models**:
  1. **Design model**: The conceptualization the designer had in mind
  2. **User's model**: What the user develops to explain system operation
  3. **System image**: System's appearance, operation, responses, documentation
- **Ideal state**: Design model and user model are identical
- **Designer's responsibility**: Ensure system image is consistent with proper conceptual model
- **Application to software**: Ideas directly applicable to digital interfaces, software UX, and websites
- **Freedom in digital**: Digital interfaces provide more freedom to work with mental model alignment than physical objects

### 3. Design Constraints and Creativity

- **2024 research** (Cromwell): Extreme levels of constraint can push people to use different creative problem-solving types
- **Combinatorial theory**: Understanding how multiple dimensions of constraint (on problems AND resources) work together
- **Two creativity-enhancing conditions**:
  1. **Divergent problem solving**: Exploring multiple solution paths
  2. **Emergent problem solving**: Solutions emerging from process itself
- **Balanced combination** of constraint improves psychological mechanisms: intrinsic motivation and creative search
- **Cross-disciplinary review** (145 studies): Some limits help people and teams generate better ideas
- **Product/design requirements** can stimulate creativity and innovation (constraints as enablers)
- **Team dynamics patterns**:
  - **Enabling dynamics**: Teams see opportunity in constraints, benefit creatively
  - **Disabling dynamics**: Constraints perceived as blockers, creativity suffers
- **Freedom in constraint**: Teams with right constraints in right environments demonstrate creative benefits

### 4. Decision Fatigue & Choice Architecture

- **Paradox of Choice**: Too many options overwhelm users and lead to decision fatigue
- **Choice architecture**: Holistic presentation and framing of information throughout decision-making process
- **2024 survey** (101 software practitioners): "Major business impact" is most challenging situation in architectural decision-making
- **Strategies to reduce decision fatigue**:
  - **Limiting choices**: Reduces cognitive load, easier decisions
  - **Progressive disclosure**: Present information step-by-step, not all at once
  - **Salience and defaults**: Highlighting best option, providing smart defaults are effective nudges
- **Choice architecture extends** beyond filtering — designing product/service to present understandable information
- **Visual hierarchy** guides user attention, reduces decision load

### 5. Code Legibility & Comprehension

- **Code readability**: What makes a program easier/harder to read and apprehend
- **Code legibility**: Ease of identifying elements of a program
- **Systematic review**: 54 relevant papers examined factors impacting developer comprehension
- **Research methods**:
  - **83.3%**: Measure correctness of subjects' results
  - **55.6%**: Ask subjects' opinions
  - **5%**: Monitor physical signs (brain activation, eye tracking)
- **Eye tracking research**: Enables objective measurement of what code parts developers read and for how long
- **Factors studied**: Programming constructs, coding idioms, naming conventions, formatting guidelines
- **Code comprehension time** generally related to readability — easier to read = less time to comprehend
- **AI impact**: Developers now spend more time reviewing code than writing it
- **Notational changes**: Seemingly insignificant changes can have profound effects on correctness and response times
- **Experience paradox**: Experience may hurt performance when underlying assumptions about code are violated

---

## Sources

### Cognitive Load Theory

1. **[Cognitive Load Theory - The Decision Lab](https://thedecisionlab.com/reference-guide/psychology/cognitive-load-theory)**
   - Core theory overview
   - Working memory limitations

2. **[The Cognitive Load Theory in Software Development](https://thevaluable.dev/cognitive-load-theory-software-developer/)**
   - Application to software engineering
   - Practical examples

3. **[Cognitive load in software engineering | Medium](https://atakde.medium.com/cognitive-load-in-software-engineering-6e9059266b79)**
   - Developer-focused analysis
   - Industry perspectives

4. **[Measuring the cognitive load of software developers | ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S095058492100046X)**
   - Systematic mapping study of 63 primary studies
   - Sensor-based measurement approaches

5. **[GitHub - zakirullin/cognitive-load](https://github.com/zakirullin/cognitive-load)**
   - Practical guide for developers
   - Code examples and patterns

6. **[Cognitive Load Theory and Individual Differences](https://www.sciencedirect.com/science/article/pii/S1041608024000165)**
   - John Sweller 2024 research
   - Optimal instructional design procedures

### Mental Models

7. **[Mental Models | Glossary of Human Computer Interaction](https://www.interaction-design.org/literature/book/the-glossary-of-human-computer-interaction/mental-models)**
   - HCI perspective on mental models
   - Don Norman's contributions

8. **[Design of Everyday Things Summary | Medium](https://medium.com/@anshikkasaini/design-of-everyday-things-by-don-norman-summary-336287b7bd73)**
   - Book summary and key concepts
   - Application to software

9. **[Don Norman - The Design of Everyday Things](https://www.sharritt.com/CISHCIExam/norman.html)**
   - Academic analysis
   - Core principles extraction

### Design Constraints and Creativity

10. **[How Combinations of Constraint Affect Creativity](https://journals.sagepub.com/doi/10.1177/20413866231202031)**
    - Johnathan R. Cromwell 2024 study
    - Combinatorial theory of constraints

11. **[Creativity and Innovation Under Constraints | ResearchGate](https://www.researchgate.net/publication/328591113_Creativity_and_Innovation_Under_Constraints_A_Cross-Disciplinary_Integrative_Review)**
    - Cross-disciplinary review of 145 studies
    - Integrative framework

12. **[Constraints Drive Innovation: 8 Examples](https://web.tapereal.com/blog/constraints-drive-innovation-8-examples/)**
    - Practical case studies
    - Industry examples

### Decision Fatigue & Choice Architecture

13. **[Choice Architecture: Introduction to Designing for Decision Making | Medium](https://zekefranco.medium.com/choice-architecture-introduction-to-designing-for-decision-making-3c2fd32cbc32)**
    - Framework overview
    - Practical application

14. **[Factors Affecting Architectural Decision-Making | Wiley](https://onlinelibrary.wiley.com/doi/10.1002/smr.2703?af=R)**
    - 2024 survey of 101 practitioners
    - Software engineering context

15. **[Decision Fatigue: The Hidden Enemy of UX | Medium](https://medium.com/design-bootcamp/decision-fatigue-the-hidden-enemy-of-user-experience-f62c061d5156)**
    - UX design perspective
    - Mitigation strategies

### Code Legibility & Comprehension

16. **[Evaluating Code Readability and Legibility | IEEE](https://ieeexplore.ieee.org/document/9240710)**
    - Systematic literature review of 54 papers
    - Human-centric studies

17. **[Code Readability Testing, an Empirical Study | ResearchGate](https://www.researchgate.net/publication/299412540_Code_Readability_Testing_an_Empirical_Study)**
    - Empirical evidence
    - Testing methodologies

18. **[Assessing Consensus of Developers' Views on Code Readability](https://arxiv.org/html/2407.03790v1)**
    - Developer perspectives
    - Consensus analysis

---

## Statistics & Data Points

### Cognitive Load

- **43% of studies** used combination of sensors to measure cognitive load — [Source 4](https://www.sciencedirect.com/science/article/abs/pii/S095058492100046X)
- **83% of studies** analyzed cognitive load during programming tasks — [Source 4](https://www.sciencedirect.com/science/article/abs/pii/S095058492100046X)
- **20% of energy** consumed by thinking while awake (cross-ref Ch 2)
- **95% of mental processing** uses fast, automatic System 1 thinking (cross-ref Ch 2)

### Design Constraints

- **145 studies reviewed** in cross-disciplinary integrative review — [Source 11](https://www.researchgate.net/publication/328591113_Creativity_and_Innovation_Under_Constraints_A_Cross-Disciplinary_Integrative_Review)
- **Balanced constraint** improves intrinsic motivation and creative search — [Source 10](https://journals.sagepub.com/doi/10.1177/20413866231202031)

### Decision Fatigue

- **101 software practitioners** surveyed on architectural decision-making (2024) — [Source 14](https://onlinelibrary.wiley.com/doi/10.1002/smr.2703?af=R)
- **"Major business impact"** identified as most challenging decision situation — [Source 14](https://onlinelibrary.wiley.com/doi/10.1002/smr.2703?af=R)

### Code Readability

- **54 relevant papers** examined in systematic review — [Source 16](https://ieeexplore.ieee.org/document/9240710)
- **83.3% of studies** measure correctness of results — [Source 16](https://ieeexplore.ieee.org/document/9240710)
- **55.6% of studies** rely on subject opinions — [Source 16](https://ieeexplore.ieee.org/document/9240710)
- **5% of studies** monitor physical signs (brain activation, eye tracking) — [Source 16](https://ieeexplore.ieee.org/document/9240710)

---

## Case Examples

### Cognitive Load in C++ vs Python

- **Context**: Comparing cognitive load across programming languages
- **Finding**: Increased cognitive load in C++ not caused by business tasks, but historical reasons (extraneous cognitive load)
- **Implication**: Language choice impacts cognitive budget for actual problem-solving
- **Source**: [Cognitive Load in Software Engineering](https://atakde.medium.com/cognitive-load-in-software-engineering-6e9059266b79)

### Mental Model Misalignment: Burbn/Instagram

- **Context**: Original app (Burbn) had too many features, confused users
- **Problem**: User's model didn't match design model — photo-sharing was used, check-in features weren't
- **Solution**: Realigned system image (Instagram) to match user's mental model — pure photo-sharing
- **Outcome**: Billion-dollar acquisition (cross-ref Ch 16 pivot research)

### Constraints Enabling Innovation: Twitter Character Limit

- **Context**: 140-character (later 280) limit on tweets
- **Constraint**: Severe limitation on message length
- **Creative outcome**: Unique communication style, threading, hashtags, brevity as feature
- **Result**: Constraint became defining characteristic and competitive advantage

### Progressive Disclosure: TurboTax

- **Context**: Complex tax software with hundreds of potential inputs
- **Decision fatigue solution**: Progressive disclosure — one question at a time
- **Outcome**: Reduced cognitive load, higher completion rates
- **Principle**: Step-by-step reveals only relevant choices based on prior answers

---

## Quotes for Book

> "Complexity is anything related to the structure of a software system that makes it hard to understand and modify the system."
> — John Ousterhout, A Philosophy of Software Design (cross-ref Ch 18)

> "Cognitive load in software engineering refers to the mental effort users spend while reading software artifacts."
> — via [Cognitive Load in Software Engineering](https://atakde.medium.com/cognitive-load-in-software-engineering-6e9059266b79)

> "Mental models are what people really have in their heads and what guides their use of things."
> — Don Norman, via [Interaction Design Foundation](https://www.interaction-design.org/literature/book/the-glossary-of-human-computer-interaction/mental-models)

> "Ideally, the design model and user model are the same, and the designer must ensure that the system image is consistent with and operates according to the proper conceptual model."
> — Don Norman, The Design of Everyday Things

> "Teams experiencing the right kinds of constraints in the right environments, and which saw opportunity in constraints, benefitted creatively from them, demonstrating that there is freedom in constraint."
> — via [Creativity and Innovation Under Constraints](https://www.researchgate.net/publication/328591113_Creativity_and_Innovation_Under_Constraints_A_Cross-Disciplinary_Integrative_Review)

> "The Paradox of Choice theory suggests that too many choices overwhelm users and lead to decision fatigue."
> — via [Decision Fatigue in UX](https://medium.com/design-bootcamp/decision-fatigue-the-hidden-enemy-of-user-experience-f62c061d5156)

> "Code comprehension time is generally related to code readability—the easier the code is to read, the less time it takes for the developer to comprehend it."
> — via [Evaluating Code Readability and Legibility](https://ieeexplore.ieee.org/document/9240710)

> "Seemingly insignificant notational changes can have profound effects on correctness and response times, and experience may hurt performance when underlying assumptions about code are violated."
> — via [Code Readability Testing](https://www.researchgate.net/publication/299412540_Code_Readability_Testing_an_Empirical_Study)

---

## Anti-Patterns to Avoid

### 1. Cognitive Overload Through Feature Bloat

- **Pattern**: Adding features without considering cumulative cognitive load on users
- **Evidence**: Burbn (pre-Instagram) had too many features, confused users
- **Cost**: User abandonment, poor adoption, support burden
- **Counter**: Progressive disclosure, feature minimalism, mental model alignment

### 2. Ignoring Extraneous Cognitive Load

- **Pattern**: Complex language/framework choices driven by resume-building, not problem fit
- **Evidence**: C++ complexity from historical reasons, not business requirements
- **Cost**: Slower development, higher error rates, difficulty onboarding
- **Counter**: Choose "boring" technology aligned with team skill and problem domain (cross-ref Ch 8 Architecture DNA)

### 3. Mental Model Misalignment

- **Pattern**: System image doesn't match either design model or user's actual mental model
- **Evidence**: User confusion, feature abandonment, workarounds
- **Cost**: Support tickets, training overhead, user frustration
- **Counter**: User research to understand mental models, align UI/terminology/flows

### 4. Unlimited Choice Without Curation

- **Pattern**: Exposing all options equally without guidance or defaults
- **Evidence**: Decision paralysis, abandonment, "analysis paralysis"
- **Cost**: Reduced conversion, user frustration, cognitive fatigue
- **Counter**: Smart defaults, progressive disclosure, salience/highlighting, constraint as feature

### 5. Constraints as Apology

- **Pattern**: Treating constraints as limitations to apologize for
- **Evidence**: Teams frame constraints negatively ("we can only...") vs opportunity ("this enables...")
- **Cost**: Missed creative opportunities, morale impact, defensive product positioning
- **Counter**: Reframe constraints as creative enablers, design boundaries as features

### 6. Inconsistent Naming/Terminology

- **Pattern**: Same concept called different things in different parts of system
- **Evidence**: Developer confusion, longer comprehension time, errors
- **Cost**: Maintenance burden, onboarding friction, bugs
- **Counter**: Ubiquitous language (DDD), style guides, code review standards (cross-ref Ch 4 MQB)

---

## Cross-References

### Related Chapters

- **Chapter 2 (HOTS)**: Dual-process cognition (System 1/2) — cognitive load connection
- **Chapter 3 (Feature Factory)**: Decision fatigue from endless backlog, no strategic filter
- **Chapter 4 (MQB)**: Code review standards reduce cognitive load via consistency
- **Chapter 7 (Experience DNA)**: Mental model alignment as MQB component
- **Chapter 8 (Architecture DNA)**: Complexity management, modularity reduces cognitive load
- **Chapter 14 (Systems/Architecture Lens)**: Deep modules hide complexity (Ousterhout reference)
- **Chapter 18 (Cognitive Load Engineering)**: Deep dive on code-specific cognitive load management

### Related Frameworks

- **Evolution Flow Cycle**: Design phase considers cognitive load of resulting features
- **Builder's Hierarchy**: Clear hierarchy reduces decision fatigue (what level am I working at?)
- **5 Lenses**: Each lens is cognitive tool — different thinking modes for different problems

### Related DNAs

- **Purpose DNA**: Constraint that enables creativity — strategic boundaries
- **User DNA**: Mental model discovery through JTBD research
- **Experience DNA**: Cognitive load as quality threshold (how hard to use?)
- **Architecture DNA**: Cognitive load on developers (how hard to maintain?)
- **Cultural DNA**: Shared mental models reduce coordination cognitive load

---

## Open Questions

1. **Cognitive Load Measurement**: How do teams practically measure cognitive load in codebases? (Complexity metrics = proxy?)

2. **Mental Model Discovery**: What research methods best uncover user mental models for complex B2B software?

3. **Constraint Calibration**: How do teams identify "right" level of constraint? (Too loose = decision fatigue; too tight = creativity stifled)

4. **Experience and Comprehension**: When does developer experience hurt vs help code comprehension? (Assumptions violated = negative transfer)

5. **Choice Architecture in Code**: Can choice architecture principles apply to API design? (Default parameters, progressive complexity?)

6. **Legibility vs Readability**: Are these truly distinct concepts, or different aspects of same underlying comprehension challenge?

---

## Next Research Steps

1. ✅ Core psychological frameworks identified (Sweller, Norman, constraints research)
2. ⏭️ **Deeper on Ousterhout** (Ch 18): A Philosophy of Software Design — complexity management techniques
3. ⏭️ **Constraint case studies**: Find 2-3 examples of constraints as features (Twitter 140-char, GitHub 80-char line limit, etc.)
4. ⏭️ **Mental model research methods**: Nielsen Norman Group, user research methodologies
5. ⏭️ **Code comprehension studies**: More recent research on naming, formatting impact
6. ⏭️ **Decision fatigue in products**: UX case studies (Amazon 1-click, Netflix recommendations, etc.)

---

**TRACE:** `RESEARCH:CH15:PSYCHOLOGICAL-CONSTRAINT:v1.0`
**Last Updated:** December 2, 2025
