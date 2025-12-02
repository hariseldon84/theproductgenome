# Chapter 20: NCO + APAP (AI Co-Creation) — Research

**Research Date:** December 2, 2025
**Researcher:** Mary (Business Analyst)
**Status:** Complete

---

## Key Findings

### 1. GitHub Copilot Effectiveness Studies

#### Productivity Impact Research

- **Communications of the ACM study** (May 2024): Analyzed 631 developer survey responses
  - **Key finding**: Acceptance rate of shown suggestions is better predictor of perceived productivity than alternative measures
  - **Implication**: Quality of suggestions matters more than quantity

- **ZoomInfo case study** (January 2025):
  - **Scale**: 400+ developers using GitHub Copilot in production
  - **Acceptance rates**: 33% for suggestions, 20% for lines (consistent across languages)
  - **Satisfaction**: 72% high satisfaction rates
  - **Cross-language consistency**: Similar performance across different programming languages

- **Automotive organization study** (August 2024):
  - **Improvements observed**: Throughput, cycle time, code quality, defects, developer satisfaction
  - **Overall impact**: Increase in developer productivity
  - **Comprehensive metrics**: Multiple dimensions measured, not just speed

- **Harness case study**:
  - **PR increase**: 10.6% increase in average number of PRs during Copilot usage month
  - **Cycle time reduction**: Average 3.5 hours, representing 2.4% improvement
  - **Measurable impact**: Quantifiable productivity gains

#### Quality Impact

- **November 2024 GitHub research**: Claims code quality gains in addition to productivity
  - **Beyond speed**: Focus shifting to quality, not just quantity
  - **Counterpoint**: Some reports show mixed results or negative findings

#### Developer Experience

- **GitHub's official research findings**:
  - **Faster completion times**: Tasks completed more quickly
  - **Mental energy conservation**: Reduces cognitive load on routine tasks
  - **Focus improvement**: Helps developers focus on more satisfying work
  - **Enjoyment**: Developers find more fun in coding with AI assistance

#### Contrarian Findings

- **Mixed results**: Not all studies show positive productivity impacts
  - Some reports answer "no" to productivity improvement question
  - **2024 DORA report** (cross-ref Ch 1): AI adoption correlated with *worse* software delivery performance for second year
  - **Nuanced reality**: Benefits not universal, depend on implementation and context

### 2. Prompt Engineering for Code Generation

#### 2024 Research Findings

- **Chain-of-thought prompting**: 43% improvement in algorithmic correctness (JAIR 2024 study)
- **GitHub Developer Survey 2024**: Developers using AI assistants generated estimated 37% of codebase through prompting
- **Microsoft 2024 Research Group**:
  - Explicit specifications reduced iterative refinement need by 68%
  - Documentation-primed prompts: 78% more likely to follow recommended patterns
- **ROI of prompting**: Better prompts dramatically improve output quality, reduce rework

#### Core Best Practices

##### 1. Specificity and Context

- **Be very specific**: More descriptive and detailed prompt = better results
- **Provide context**: Background information improves relevance
- **Define requirements**: Clearly state expected behavior

##### 2. Examples and Few-Shot Learning

- **Dramatic improvement**: Examples significantly boost code generation quality
- **Pattern following**: Small samples help when generating code following specific conventions
- **Chain-of-thought + few-shot**: Combination identified as best practice

##### 3. Iterative Refinement

- **Design as iterative process**: Requires experimentation for optimal results
- **Continuous improvement**: Iterate prompt along the way
- **Feedback loops**: Use output quality to refine next prompts

##### 4. Code-Specific Guidance

- **Describe outcome**: Be descriptive about desired result
- **Specify language**: Include programming language in prompt
- **Structural hints**: Guide with class names, field names, structure
- **Define capabilities**: Specify traits, base class, interface, other requirements

### 3. Human-AI Collaboration Patterns

#### Collaboration Model Evolution

- **Shift in thinking**: From "AI as tool" to "AI as teammate"
- **New governance needs**: Requires policies for human-AI collaboration, supervision models, accountability frameworks
- **Employee-like nature**: Agent systems require more sophisticated governance than simple tools

#### Adoption Statistics

- **Stack Overflow survey**: 76% of developers using or interested in AI tools
- **GitHub enterprise survey**: Almost every enterprise respondent has used AI coding tools at work
- **Widespread adoption**: AI assistance becoming standard practice

#### Strategic Skill: Prompt Engineering

- **New core competency**: Shapes how developers and AI systems collaborate
- **Dual impact**: Affects individual productivity AND team-based workflows
- **Career evolution**: Prompt engineering as strategic skill for developers

#### Complementary Strengths

- **AI excels at**: Pattern recognition, maintaining consistency, routine tasks
- **Humans remain superior in**: Creative problem-solving, ethical decision-making, strategic thinking
- **Effective collaboration**: Leveraging complementary strengths, not replacement

#### New Skills Required

- **Directing AI tools**: Developers need to learn how to guide AI effectively
- **Evaluating outputs**: Critical assessment of AI-generated code
- **Integration skills**: Incorporating AI suggestions into coherent solutions

#### Research Gaps

- **Longitudinal studies**: Lack of long-term impact research
- **Personalization strategies**: How to customize AI assistance per developer
- **Development-specific governance**: Frameworks still emerging

### 4. AI Governance Frameworks (2024)

#### Regulatory Landscape

- **EU Artificial Intelligence Act**: Passed into law 2024 after years of debate
  - Expected to influence similar laws in other regions (like GDPR did)
- **AI Safety Institutes**: New in 2024 in US, UK, Singapore, Japan
- **EU AI Office**: Established under EU AI Act
- **Global coordination**: Increasing focus on AI safety and governance

#### Governance Principles

- **Clear policies needed**: For human-AI collaboration in development contexts
- **Supervision models**: How to oversee AI-generated code
- **Accountability frameworks**: Who's responsible for AI outputs
- **Quality gates**: Special considerations for AI-generated artifacts (cross-ref Ch 4 MQB)

---

## Sources

### GitHub Copilot Effectiveness

1. **[Research: Quantifying GitHub Copilot's Impact | GitHub Blog](https://github.blog/news-insights/research/research-quantifying-github-copilots-impact-on-developer-productivity-and-happiness/)**
   - Official GitHub research
   - Productivity and happiness metrics

2. **[Impact of GitHub Copilot on Developer Productivity | ResearchGate](https://www.researchgate.net/publication/381609417_The_impact_of_GitHub_Copilot_on_developer_productivity_from_a_software_engineering_body_of_knowledge_perspective)**
   - Academic perspective
   - Software engineering body of knowledge

3. **[Measuring Impact of GitHub Copilot | GitHub Resources](https://resources.github.com/learn/pathways/copilot/essentials/measuring-the-impact-of-github-copilot/)**
   - Official measurement guide
   - Enterprise adoption

4. **[Measuring GitHub Copilot's Impact on Productivity | ACM](https://cacm.acm.org/research/measuring-github-copilots-impact-on-productivity/)**
   - May 2024 research study
   - 631 developer responses

5. **[GitHub Copilot Dev Productivity Report | Visual Studio Magazine](https://visualstudiomagazine.com/articles/2024/09/17/another-report-weighs-in-on-github-copilot-dev-productivity.aspx)**
   - Critical perspective
   - Contrarian findings

6. **[GitHub Copilot Code Quality Research | Visual Studio Magazine](https://visualstudiomagazine.com/articles/2024/11/22/article_0github-copilot-research-claims-code-quality-gains-in-addition-to-productivity.aspx)**
   - November 2024 quality claims
   - Beyond productivity focus

7. **[GitHub Copilot Developer Productivity Case Study | Harness](https://www.harness.io/blog/the-impact-of-github-copilot-on-developer-productivity-a-case-study)**
   - Enterprise case study
   - Quantified metrics

8. **[Experience with GitHub Copilot at ZoomInfo | arXiv](https://arxiv.org/html/2501.13282v1)**
   - January 2025 study
   - 400+ developers

### Prompt Engineering

9. **[Prompt Engineering for Code Generation | Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)**
   - Best practices guide
   - Code-specific techniques

10. **[PromptHub: Prompt Engineering Principles for 2024](https://www.prompthub.us/blog/prompt-engineering-principles-for-2024)**
    - 2024 updated principles
    - Current best practices

11. **[GitHub - DAIR.AI Prompt Engineering Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)**
    - Comprehensive open-source guide
    - Community-driven best practices

12. **[The Ultimate Guide to Prompt Engineering 2025 | Lakera](https://www.lakera.ai/blog/prompt-engineering-guide)**
    - 2025 perspective
    - Security considerations

13. **[Best Practices for Prompt Engineering | OpenAI](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api)**
    - Official OpenAI guidance
    - API-specific techniques

14. **[Prompt Engineering Best Practices | DigitalOcean](https://www.digitalocean.com/resources/articles/prompt-engineering-best-practices)**
    - Practical implementation
    - Tips and tools

15. **[Prompt Engineering in 2025: Latest Best Practices](https://www.news.aakashg.com/p/prompt-engineering)**
    - Most recent updates
    - Emerging patterns

### Human-AI Collaboration & Governance

16. **[From Assistant to Agent: Governing Autonomous AI | Credo AI](https://www.credo.ai/recourseslongform/from-assistant-to-agent-navigating-the-governance-challenges-of-increasingly-autonomous-ai)**
    - Governance evolution
    - Autonomy challenges

17. **[Guide Towards Collaborative AI Frameworks | Digital Regulation Platform](https://digitalregulation.org/a-guide-towards-collaborative-ai-frameworks/)**
    - Regulatory perspective
    - Framework overview

18. **[Human-AI Teaming in Age of Collaborative Intelligence | SecureWorld](https://www.secureworld.io/industry-news/human-ai-teaming-age-collaboration)**
    - Team dynamics
    - Collaboration patterns

19. **[6 AI-Human Development Collaboration Models | Augment Code](https://www.augmentcode.com/guides/6-ai-human-development-collaboration-models-that-work)**
    - Practical models
    - What works in practice

20. **[Human-AI Experience in IDEs: Systematic Literature Review | arXiv](https://arxiv.org/html/2503.06195v1)**
    - Comprehensive academic review
    - Research gaps identified

21. **[AI Governance Trends 2024 | World Economic Forum](https://www.weforum.org/stories/2024/09/ai-governance-trends-to-watch/)**
    - Global governance landscape
    - 2024 regulatory updates

---

## Statistics & Data Points

### Productivity Impact

- **631 developer responses** analyzed in ACM study — [Source 4](https://cacm.acm.org/research/measuring-github-copilots-impact-on-productivity/)
- **400+ developers** using Copilot at ZoomInfo — [Source 8](https://arxiv.org/html/2501.13282v1)
- **33% acceptance rate** for suggestions, **20% for lines** — [Source 8](https://arxiv.org/html/2501.13282v1)
- **72% high satisfaction** rates — [Source 8](https://arxiv.org/html/2501.13282v1)
- **10.6% increase** in average PRs during Copilot month — [Source 7](https://www.harness.io/blog/the-impact-of-github-copilot-on-developer-productivity-a-case-study)
- **3.5 hours reduction** in cycle time (2.4% improvement) — [Source 7](https://www.harness.io/blog/the-impact-of-github-copilot-on-developer-productivity-a-case-study)

### Prompt Engineering Impact

- **43% improvement** in algorithmic correctness (chain-of-thought prompting, 2024 JAIR study) — [Source 9](https://margabagus.com/prompt-engineering-code-generation-practices/)
- **37% of codebase** generated through AI prompting (GitHub 2024 survey) — [Source 9](https://margabagus.com/prompt-engineering-code-generation-practices/)
- **68% reduction** in need for iterative refinement (explicit specifications, Microsoft 2024) — [Source 9](https://margabagus.com/prompt-engineering-code-generation-practices/)
- **78% more likely** to follow recommended patterns (documentation-primed prompts, Microsoft 2024) — [Source 9](https://margabagus.com/prompt-engineering-code-generation-practices/)

### Adoption

- **76% of developers** using or interested in AI tools (Stack Overflow) — [Source 18](https://www.secureworld.io/industry-news/human-ai-teaming-age-collaboration)
- **Almost every enterprise** respondent used AI coding tools at work (GitHub survey) — [Source 18](https://www.secureworld.io/industry-news/human-ai-teaming-age-collaboration)

---

## Case Examples

### ZoomInfo: Enterprise Copilot Deployment

- **Context**: 400+ developers, production deployment
- **Acceptance rates**: 33% suggestions, 20% lines (consistent across languages)
- **Satisfaction**: 72% high satisfaction
- **Key insight**: Consistent performance across programming languages suggests broad applicability
- **Source**: [arXiv Study](https://arxiv.org/html/2501.13282v1)

### Harness: Quantified Productivity Gains

- **Metric 1**: 10.6% increase in average PRs
- **Metric 2**: 3.5 hour reduction in cycle time (2.4% improvement)
- **Approach**: Controlled before/after comparison
- **Lesson**: Measurable productivity gains when properly instrumented
- **Source**: [Harness Blog](https://www.harness.io/blog/the-impact-of-github-copilot-on-developer-productivity-a-case-study)

### Chain-of-Thought Prompting: Algorithmic Correctness

- **Context**: Solving algorithmic problems with AI assistance
- **Approach**: Chain-of-thought prompting (explain reasoning step-by-step)
- **Result**: 43% improvement in correctness
- **Lesson**: Prompt engineering technique significantly impacts output quality
- **Source**: [JAIR 2024 via Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)

### Microsoft Research: Documentation-Primed Prompts

- **Finding**: Prompts referencing documentation → 78% more likely to follow best practices
- **Implication**: Context matters enormously in code generation
- **Application**: Include relevant documentation snippets in prompts
- **Source**: [Microsoft 2024 Research via Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)

---

## Quotes for Book

> "Acceptance rate of shown suggestions is a better predictor of perceived productivity than alternative measures."
> — ACM Study (May 2024), via [ACM](https://cacm.acm.org/research/measuring-github-copilots-impact-on-productivity/)

> "GitHub Copilot supports faster completion times, conserves developers' mental energy, helps them focus on more satisfying work, and ultimately find more fun in the coding they do."
> — GitHub Official Research, via [GitHub Blog](https://github.blog/news-insights/research/research-quantifying-github-copilots-impact-on-developer-productivity-and-happiness/)

> "Chain-of-thought prompting resulted in a 43% improvement in algorithmic correctness according to a 2024 study published in the Journal of Artificial Intelligence Research."
> — via [Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)

> "In 2024, developers using AI coding assistants generated an estimated 37% of their codebase through prompt engineering techniques, according to GitHub's Developer Survey."
> — via [Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)

> "Prompts with explicit specifications reduced the need for iterative refinement by 68%. Documentation-primed prompts resulted in code that was 78% more likely to follow recommended patterns."
> — Microsoft 2024 Developer Tools Research Group, via [Margabagus](https://margabagus.com/prompt-engineering-code-generation-practices/)

> "AI governance is experiencing a shift from 'AI as tool' to 'AI as teammate' thinking, requiring more sophisticated governance that addresses the employee-like nature of agent systems, with clear policies for human-AI collaboration, supervision models, and accountability frameworks."
> — via [Credo AI](https://www.credo.ai/recourseslongform/from-assistant-to-agent-navigating-the-governance-challenges-of-increasingly-autonomous-ai)

> "AI excels at pattern recognition and maintaining consistency, while humans remain superior in creative problem-solving and ethical decision-making."
> — via [SecureWorld](https://www.secureworld.io/industry-news/human-ai-teaming-age-collaboration)

> "Prompt engineering is positioned as a strategic skill that shapes how developers and AI systems collaborate, affecting both individual productivity and team-based workflows."
> — via [Augment Code](https://www.augmentcode.com/guides/6-ai-human-development-collaboration-models-that-work)

---

## Anti-Patterns to Avoid

### 1. Blind Acceptance of AI Suggestions

- **Pattern**: Accepting all AI suggestions without critical review
- **Evidence**: Quality issues, security vulnerabilities, logic errors
- **Cost**: Technical debt, production bugs, security incidents
- **Counter**: Critical evaluation, code review for AI-generated code (MQB applies, Ch 4)

### 2. No Prompt Engineering Training

- **Pattern**: Expecting developers to be effective with AI without guidance
- **Evidence**: Low acceptance rates, poor quality output, frustration
- **Cost**: Underutilized tools, wasted license costs, missed productivity gains
- **Counter**: Prompt engineering training, shared best practices, internal documentation

### 3. Treating AI as Infallible

- **Pattern**: Assuming AI understands requirements and context perfectly
- **Evidence**: Misaligned implementations, incorrect assumptions
- **Cost**: Rework, bugs, misaligned features
- **Counter**: Iterative prompting, validation, human oversight

### 4. No Governance Framework

- **Pattern**: Ad-hoc AI usage without policies or standards
- **Evidence**: Inconsistent code quality, security risks, IP concerns
- **Cost**: Compliance violations, security vulnerabilities, legal exposure
- **Counter**: AI governance framework (policies, standards, accountability)

### 5. Ignoring Contrarian Research

- **Pattern**: Assuming AI tools always improve productivity
- **Evidence**: DORA 2024 — AI adoption correlated with worse performance
- **Cost**: Misallocated resources, false productivity assumptions
- **Counter**: Measure actual impact in your context, not just trust vendor claims

### 6. AI Replacing Human Judgment

- **Pattern**: Using AI for strategic decisions requiring judgment
- **Evidence**: Poor architectural decisions, ethical issues, context-ignorant choices
- **Cost**: Technical debt, misaligned product direction
- **Counter**: AI for pattern recognition, humans for strategy/ethics/creativity

---

## Cross-References

### Related Chapters

- **Chapter 1 (Chaos)**: DORA 2024 — AI adoption correlating with worse performance
- **Chapter 2 (HOTS)**: AI as tool requiring structured thinking to use effectively
- **Chapter 4 (MQB)**: Quality gates for AI-generated code
- **Chapter 8 (Architecture DNA)**: AI governance as architectural decision
- **Chapter 15 (Psychological Lens)**: Cognitive load — AI reducing routine cognitive burden
- **Chapter 18 (Cognitive Load Engineering)**: Ousterhout — AI design importance increasing

### Related Frameworks

- **MQB Components**: AI-generated code must meet same standards (tests, review, security)
- **Evolution Flow**: AI assists in Design and Build phases, requires Validation
- **Builder's Hierarchy**: AI generates features/tasks, humans define outcomes/capabilities

### Related DNAs

- **Architecture DNA**: Governance frameworks, where AI fits in system
- **Data DNA**: Prompt context, training data, feedback loops
- **Validation DNA**: Testing AI outputs, measuring effectiveness
- **Cultural DNA**: Ethical AI use, responsible automation

---

## Open Questions

1. **Long-term Impact**: Do productivity gains persist over months/years, or habituate?

2. **Skill Evolution**: How does AI change what skills developers need? (Prompt engineering vs traditional coding)

3. **Code Quality Trajectory**: Does AI-generated code improve or degrade over time as models evolve?

4. **Governance Standards**: What standards/frameworks will emerge for AI code governance? (Industry consensus?)

5. **Liability**: Who's responsible for bugs in AI-generated code? (Developer? Company? AI vendor?)

6. **NCO + APAP Specifics**: User wants NCO + APAP explained — need to clarify what these acronyms mean in their context

7. **Personalization**: Can AI assistance be personalized per developer? (Learning individual preferences/styles)

---

## Next Research Steps

1. ✅ Core AI effectiveness research gathered (GitHub Copilot studies)
2. ✅ Prompt engineering best practices documented
3. ✅ Governance frameworks surveyed
4. ⏭️ **NCO + APAP clarification**: Understand user's specific meaning for these terms
5. ⏭️ **Deeper case studies**: More enterprise examples of successful AI integration
6. ⏭️ **AI governance frameworks**: Detailed standards (IEEE, ISO emerging?)
7. ⏭️ **Longitudinal studies**: Find multi-year impact research (if available)
8. ⏭️ **AI pair programming**: Copilot alternatives (Cursor, Tabnine, Codeium), comparative studies

---

**TRACE:** `RESEARCH:CH20:NCO-APAP-AI:v1.0`
**Last Updated:** December 2, 2025
