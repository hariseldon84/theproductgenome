# Prompting Playbook

**Project:** [Project Name]  
**Last Updated:** [YYYY-MM-DD]  
**Maintained By:** [Team/Role]

---

## Purpose

Document effective prompting strategies, patterns, and anti-patterns for collaborating with AI agents, enabling consistent, high-quality AI-human co-creation.

---

## Prompting Framework

**Effective prompts follow the CRAFT structure:**

- **C**ontext: Background and situation
- **R**ole: What perspective the AI should take
- **A**ction: What you want the AI to do
- **F**ormat: How the output should be structured
- **T**one: Style and audience considerations

---

## Prompt Patterns Library

### Pattern 1: Artifact Generation

**Use Case:** Generate PRDs, user stories, architecture docs, test plans

**Template:**
```
[CONTEXT]
We are building [product/feature description]. Our users are [personas] who need to [JTBD]. We currently have [existing functionality]. Key constraints: [technical, business, timeline constraints].

[ROLE]
Act as a [Product Manager/Architect/Developer/QA] with expertise in [domain].

[ACTION]
Create a [artifact type] for [specific feature/component]. Include:
- [Section 1]
- [Section 2]
- [Section 3]

[FORMAT]
Use markdown with headings, tables, and bullet lists. Structure as:
1. [Section 1]
2. [Section 2]
...

[TONE]
Clear, concise, actionable. Target audience: [who will use this].
```

**Example:**
```
[CONTEXT]
We are building a task management SaaS. Our users are small teams (5-20 people) who need to coordinate work without heavy process. We currently have basic task creation and assignment. Key constraints: must integrate with Slack, launch in 6 weeks.

[ROLE]
Act as a Product Manager with expertise in productivity tools and SaaS.

[ACTION]
Create a PRD for a "Task Dependencies" feature that allows users to link tasks and see what's blocking what. Include:
- User stories
- Acceptance criteria
- Edge cases
- Success metrics

[FORMAT]
Use markdown with H2 for sections, tables for acceptance criteria, bullet lists for edge cases.

[TONE]
Clear, concise, actionable. Target audience: engineering team implementing this feature.
```

---

### Pattern 2: Analysis & Insights

**Use Case:** Analyze data, feedback, metrics; identify patterns

**Template:**
```
[CONTEXT]
[Description of what data/information you're analyzing and why]

[ROLE]
Act as a [data analyst/user researcher/technical architect] with expertise in [domain].

[ACTION]
Analyze [data/feedback/metrics] to:
- [Goal 1: e.g., identify top pain points]
- [Goal 2: e.g., find patterns]
- [Goal 3: e.g., recommend actions]

[FORMAT]
Provide:
1. Summary of findings (top 3-5 insights)
2. Supporting evidence
3. Recommended actions with priority

[TONE]
Data-driven, objective, with clear reasoning for conclusions.
```

**Example:**
```
[CONTEXT]
We launched a new onboarding flow 2 weeks ago. Completion rate dropped from 80% to 60%. We have Mixpanel event data and user feedback from 50 users.

[ROLE]
Act as a user researcher and UX analyst with expertise in onboarding optimization.

[ACTION]
Analyze the provided data to:
- Identify where users are dropping off
- Understand why (from feedback)
- Recommend fixes prioritized by impact

[FORMAT]
Provide:
1. Drop-off analysis (funnel visualization if possible)
2. User feedback themes
3. Recommended fixes with estimated impact and effort

[TONE]
Data-driven, objective, actionable for product and engineering teams.
```

---

### Pattern 3: Iteration & Refinement

**Use Case:** Improve AI-generated drafts

**Template:**
```
[CONTEXT]
You previously generated [artifact]. Here's my feedback: [specific feedback].

[ACTION]
Revise [artifact] to address:
- [Feedback point 1]
- [Feedback point 2]
- [Feedback point 3]

[FORMAT]
Show me:
1. What you changed (diff or summary)
2. Updated artifact
3. Rationale for changes

[TONE]
[Same as original or specify changes]
```

**Example:**
```
[CONTEXT]
You previously generated a user story for task dependencies. Here's my feedback:
- The acceptance criteria are too technical and not user-focused
- Missing edge case: what happens if circular dependencies are created
- Success metrics should include adoption rate, not just completion

[ACTION]
Revise the user story to address these points.

[FORMAT]
Show me:
1. Summary of changes
2. Updated user story
3. Why you made these changes

[TONE]
Same as before: clear, concise, actionable for engineers.
```

---

### Pattern 4: Options & Trade-offs

**Use Case:** Explore alternatives, compare approaches

**Template:**
```
[CONTEXT]
[Situation and decision to be made]

[ROLE]
Act as a [strategist/architect/designer] with expertise in [domain].

[ACTION]
Provide 3-5 options for [decision/approach], for each option include:
- Description
- Pros
- Cons
- Estimated effort/cost
- Risk level

Then recommend one option with clear rationale.

[FORMAT]
Table or structured list for easy comparison.

[TONE]
Objective, balanced, with clear reasoning for recommendation.
```

**Example:**
```
[CONTEXT]
We need to add real-time notifications to our app. Users expect instant updates when tasks are assigned or commented on. We have ~10K users, growing 20%/month.

[ROLE]
Act as a technical architect with expertise in real-time systems and scalability.

[ACTION]
Provide 3-5 options for implementing real-time notifications. For each:
- Technology/approach
- Pros
- Cons
- Estimated effort (eng-weeks)
- Scalability & cost

Then recommend one option with rationale.

[FORMAT]
Table for comparison, followed by recommendation paragraph.

[TONE]
Objective, technical, for engineering leadership decision.
```

---

### Pattern 5: Validation & Review

**Use Case:** Check artifacts for completeness, quality, consistency

**Template:**
```
[CONTEXT]
[Description of artifact and its purpose]

[ROLE]
Act as a [reviewer type: QA, architect, PM] with a focus on [quality dimension: completeness, security, usability].

[ACTION]
Review [artifact] and identify:
- What's missing
- What's unclear or ambiguous
- What's inconsistent with [standards/guidelines]
- Risks or edge cases not addressed

[FORMAT]
Provide:
1. Summary (pass/fail, overall assessment)
2. Detailed findings categorized by severity (critical/important/minor)
3. Recommended fixes

[TONE]
Constructive, specific, actionable.
```

**Example:**
```
[CONTEXT]
Here's a PRD for task dependencies feature. It needs to align with our technical architecture (microservices, REST API, React frontend) and be ready for engineering to implement.

[ROLE]
Act as a Technical Architect reviewing this PRD for technical feasibility and completeness.

[ACTION]
Review the PRD and identify:
- Missing technical details
- Unclear or ambiguous requirements
- Inconsistencies with our architecture
- Risks or technical debt implications

[FORMAT]
Provide:
1. Summary (ready for dev? Y/N)
2. Critical issues (must fix before dev)
3. Important issues (should fix)
4. Minor improvements (nice to have)

[TONE]
Constructive, specific, with actionable recommendations.
```

---

### Pattern 6: Brainstorming & Ideation

**Use Case:** Generate ideas, explore possibilities

**Template:**
```
[CONTEXT]
[Problem or opportunity to explore]

[ROLE]
Act as a creative [strategist/designer/innovator] with expertise in [domain].

[ACTION]
Brainstorm [N] ideas for [problem/opportunity]. For each idea:
- Concept (1-2 sentences)
- Why it might work
- Potential challenges
- Rough effort estimate

No filtering yet—focus on quantity and variety.

[FORMAT]
Numbered list or table.

[TONE]
Creative, open-minded, exploratory.
```

**Example:**
```
[CONTEXT]
Our task management app has good retention but low viral growth. We want to increase organic user acquisition without paid ads.

[ROLE]
Act as a growth strategist with expertise in B2B SaaS viral loops.

[ACTION]
Brainstorm 10 ideas for increasing organic user acquisition. For each:
- Concept
- Why it might work
- Challenges
- Rough effort (low/med/high)

Focus on variety—include both incremental and bold ideas.

[FORMAT]
Numbered list with columns: Idea | Why | Challenges | Effort

[TONE]
Creative, optimistic, exploratory.
```

---

## Prompting Best Practices

### ✅ DO

1. **Provide Context:** Always explain the situation, constraints, and goals
2. **Be Specific:** "Create a user story for task dependencies" > "write a story"
3. **Define Format:** Specify structure, sections, and level of detail
4. **Show Examples:** Include sample outputs or references when possible
5. **Iterate:** Start broad, then refine with follow-up prompts
6. **Request Reasoning:** Ask AI to explain its logic and trade-offs
7. **Set Boundaries:** Explicitly state what NOT to do
8. **Use Structured Templates:** CRAFT framework for consistency
9. **Break Down Complex Tasks:** Multiple prompts > one giant prompt
10. **Reference Standards:** Point to existing docs, patterns, or conventions

### ❌ DON'T

1. **Assume Context:** AI doesn't know your project, users, or constraints unless told
2. **Be Vague:** "Make it better" is unhelpful; specify what to improve
3. **Skip Format Instructions:** Unstructured output is harder to use
4. **Accept First Draft:** Always review and iterate
5. **Expect Perfection:** AI will need guidance and refinement
6. **Over-Rely on AI:** AI augments, doesn't replace human judgment
7. **Ignore Hallucinations:** Verify facts, especially technical details
8. **Reuse Same Prompt Forever:** Update prompts as you learn what works
9. **Mix Multiple Goals:** One prompt = one clear objective
10. **Forget to Document:** Save effective prompts for team reuse

---

## Role-Specific Prompting Guides

### For Product Managers

**Common Tasks:**
- Writing PRDs
- Analyzing user feedback
- Prioritizing features
- Creating roadmaps

**Effective Prompts:**
- Always include user personas and JTBD
- Reference existing product context
- Request options and trade-offs
- Ask for success metrics

**Example Library:**
- [Link to PM prompt examples]

---

### For Architects

**Common Tasks:**
- Designing systems
- Reviewing technical proposals
- Creating architecture docs
- Evaluating technologies

**Effective Prompts:**
- Specify technical constraints (scale, latency, budget)
- Reference existing architecture
- Request trade-off analysis
- Ask for failure modes and mitigations

**Example Library:**
- [Link to architecture prompt examples]

---

### For Developers

**Common Tasks:**
- Code generation/refactoring
- Test case creation
- Bug analysis
- Performance optimization

**Effective Prompts:**
- Provide relevant code context
- Specify coding standards
- Request tests with code
- Ask for edge cases

**Example Library:**
- [Link to dev prompt examples]

---

### For QA/Test Engineers

**Common Tasks:**
- Test plan creation
- Test case generation
- Bug reproduction
- Quality assessment

**Effective Prompts:**
- Include acceptance criteria
- Reference testing standards
- Request edge cases and negative tests
- Ask for test data requirements

**Example Library:**
- [Link to QA prompt examples]

---

## Anti-Patterns (What NOT to Do)

| Anti-Pattern | Why It Fails | Better Approach |
|-------------|-------------|-----------------|
| **"Write a PRD"** | Too vague, no context | Use Pattern 1 with full CRAFT structure |
| **"Make it perfect"** | Subjective, no criteria | Specify quality dimensions: "Ensure all ACs have testable criteria" |
| **"Fix this code"** | No indication what's wrong | "Refactor this function to reduce cyclomatic complexity from 15 to <10" |
| **One massive prompt** | Overwhelming, unfocused | Break into sequential prompts, each with clear goal |
| **No review process** | Accept AI output blindly | Always review, validate, iterate |
| **Reusing outdated prompt** | Context changed, prompt didn't | Update prompts as project evolves |

---

## Prompt Versioning

**Track and improve prompts over time:**

| Prompt ID | Purpose | Version | What Changed | Effectiveness | Date |
|-----------|---------|---------|--------------|---------------|------|
| PM-PRD-01 | Generate PRD | v1 | Initial | 60% approval rate | [Date] |
| PM-PRD-01 | Generate PRD | v2 | Added technical constraints section | 85% approval rate | [Date] |

**Improvement Process:**
1. Use prompt, measure effectiveness (approval rate, iteration count)
2. Identify failure modes (what's missing, what's wrong)
3. Update prompt to address failures
4. Re-test and measure improvement
5. Share updated prompt with team

---

## Contextual Prompts for Different Stages

### Vision Stage (Layer 2)

**Focus:** Exploration, ideation, problem definition

**Prompt Style:** Open-ended, brainstorming, multiple options

**Example:**
"Brainstorm 10 ways we could improve task collaboration for remote teams. Focus on problems users face with async communication."

---

### Decomposition Stage (Layer 2)

**Focus:** Breaking down into features, defining scope

**Prompt Style:** Structured, analytical, hierarchical

**Example:**
"Decompose the 'Task Dependencies' feature into 3-5 user stories. For each story, include JTBD, acceptance criteria, and estimated complexity."

---

### Design Stage (Layer 2)

**Focus:** Technical/UX design, architecture, trade-offs

**Prompt Style:** Detailed, with constraints and standards

**Example:**
"Design the API for task dependencies. Include endpoints, request/response schemas, error handling. Must align with our REST conventions and support optimistic UI updates."

---

### Build Stage (Layer 2)

**Focus:** Implementation, testing, code quality

**Prompt Style:** Specific, technical, with examples

**Example:**
"Generate unit tests for the TaskDependency model. Cover happy path, edge cases (circular deps, orphaned tasks), and validation errors. Follow our Jest conventions."

---

### Validate Stage (Layer 2)

**Focus:** Testing, metrics, analysis

**Prompt Style:** Analytical, data-driven, quality-focused

**Example:**
"Analyze these A/B test results for task dependencies feature. Determine if we met our success criteria (+10% task completion rate). Recommend ship/iterate/kill."

---

### Evolve Stage (Layer 2)

**Focus:** Optimization, scaling, iteration

**Prompt Style:** Improvement-focused, forward-looking

**Example:**
"Review the task dependencies feature post-launch. Identify: (1) what's working well, (2) common user complaints, (3) opportunities to increase adoption. Prioritize improvements."

---

## Advanced Prompting Techniques

### Chain-of-Thought Prompting

**Technique:** Ask AI to reason step-by-step

**Example:**
"Before recommending an architecture, think through:
1. What are the key requirements?
2. What are the constraints?
3. What are 3 possible approaches?
4. What are the trade-offs of each?
5. Based on this analysis, what do you recommend?"

### Few-Shot Prompting

**Technique:** Provide examples of desired output

**Example:**
"Create user stories like these examples:
[Example 1]
[Example 2]
Now create a story for [new feature]."

### Role Prompting

**Technique:** Assign a specific expert role to AI

**Example:**
"Act as a senior technical architect with 10 years experience in distributed systems. Review this design..."

### Constraint Prompting

**Technique:** Define what NOT to do

**Example:**
"Design this API. Constraints: Do NOT use GraphQL (we're REST-only). Do NOT add new database tables (use existing Task model). Do NOT require real-time updates (polling is OK)."

---

## Prompt Debugging

**If AI output is poor:**

1. **Check Context:** Did you provide enough background?
2. **Check Specificity:** Is your request clear and specific?
3. **Check Format:** Did you specify the output structure?
4. **Check Examples:** Would an example help clarify?
5. **Check Constraints:** Did you state what NOT to do?
6. **Iterate:** Refine the prompt and try again

**Common Fixes:**
- "Too generic" → Add more context and constraints
- "Wrong format" → Specify structure explicitly
- "Misunderstood goal" → Clarify action and success criteria
- "Hallucinated facts" → Ask for source references
- "Too verbose" → Request concise output with specific sections

---

## Team Prompt Library

**Store reusable prompts:**

- **Location:** [Notion/Confluence/GitHub/etc.]
- **Organization:** By role (PM/Arch/Dev/QA) and task type
- **Versioning:** Track effectiveness, update as needed
- **Contribution:** Team members add new prompts and improvements

**Library Structure:**
```
/prompt-library
  /product-management
    - prd-generation.md
    - user-story-creation.md
    - feature-prioritization.md
  /architecture
    - system-design.md
    - api-design.md
    - tech-evaluation.md
  /development
    - code-generation.md
    - refactoring.md
    - test-creation.md
  /qa
    - test-plan.md
    - bug-analysis.md
    - quality-review.md
```

---

## Review & Updates

**Monthly:**
- Review prompt effectiveness metrics (approval rates, iteration counts)
- Identify low-performing prompts
- Update prompts based on learnings

**Quarterly:**
- Team workshop: share best prompts, anti-patterns discovered
- Update playbook with new patterns
- Sunset ineffective prompts

---

**TRACE:** L4:NCO:Prompting  
**Cross-ref:** Collaboration Charter, Decision Journal, Evolve Stage (L2), Cultural DNA (L1)
