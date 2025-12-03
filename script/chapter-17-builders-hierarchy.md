# Chapter 17: Builder's Hierarchy

**TRACE:** `SCRIPT:PART4:CH17:v1.0`

---

Rachel, the VP of Product at CloudOps (a DevOps platform with 200 engineers), walked into the quarterly review with the CEO and Board. The team had shipped 47 features in Q3—the highest velocity in company history. The engineering dashboard showed green. The product team was proud.

Then the CEO asked: **"Which of these 47 features moved our North Star Metric?"**

Silence.

Rachel pulled up the North Star dashboard: **Monthly Active Teams remained flat**. Retention hadn't budged. The features customers actually wanted—better alerting, faster deployments—hadn't shipped. What did ship? Features requested by individual customers, features from sales escalations, features engineers wanted to build.

**47 features. Zero strategic impact.**

The problem wasn't execution—it was **strategic disconnect**. No one could answer: **"Why are we building this? Which business outcome does it serve? Which user need does it address?"** Features existed in a backlog, disconnected from strategy.

Rachel realized they needed what she'd call the **Builder's Hierarchy**—a framework connecting **strategic outcomes** (top) to **features** (middle) to **tasks** (bottom), ensuring every line of code traced to a business goal.

---

## The Hierarchy Problem: Strategic Drift

Most organizations suffer from **strategic drift**—the gradual misalignment between what leadership intends and what teams build. This happens when there's no **explicit, enforced hierarchy** connecting strategy to execution.

### The Symptom: Feature Backlogs as Shopping Lists

Gojko Adzic, in *Impact Mapping*, observed: **"Most planning activities revolve around juggling a 'shopping list of features,' and even though the features are delivered, often the business objective is not achieved"** (1).

**Why does this happen?**

1. **Features enter backlogs** from multiple sources: customer requests, sales promises, executive ideas, competitive analysis, engineering proposals
2. **Priority becomes political**, not strategic—whoever shouts loudest wins
3. **Teams optimize for throughput** (features shipped) not outcomes (value delivered)
4. **No one can kill features**—everything is "important" because someone requested it

The result: **80% of features go unused** (Chapter 1), not because they're poorly built, but because they don't align with actual user needs or business goals.

### The Solution: Hierarchical Traceability

**Impact Mapping** provides a structured hierarchy that **reorients teams towards delivering value, not delivering features** (2). It addresses common problems:
- Wrong assumptions
- Lack of focus
- Poor communication of objectives
- Lack of understanding
- Misalignment with overall goals (3)

The hierarchy ensures every deliverable traces to an impact, which traces to an actor, which traces to a goal. **If you can't trace it, don't build it.**

---

## Impact Mapping: The Four-Level Hierarchy

Impact Mapping, created by Gojko Adzic, structures product planning around **outcomes, not outputs** (3, 4). The hierarchy has four levels:

### Level 1: Goal (Why?)

**The business objective you're trying to achieve.**

Not "build a dashboard" or "add analytics"—that's an output. The goal is **why you want those things**. Example goals:
- Increase Monthly Active Teams by 25% in Q4
- Reduce churn from 5% to 3% within 6 months
- Enable enterprise customers to self-serve 80% of support requests

**Characteristics of good goals**:
- **Measurable**: You'll know when you've achieved it
- **Time-bound**: Deadline creates urgency
- **Business-focused**: Expressed in business or user value terms, not features

### Level 2: Actors (Who?)

**Who can produce the desired effect? Whose behavior change would help achieve the goal?**

Actors are **user segments** (aligns with **User DNA**, Chapter 6). Don't say "users"—be specific. Examples:
- Team leads (who decide whether to adopt the tool)
- DevOps engineers (who configure and maintain it)
- Executives (who approve budget)

**Key insight**: Different actors need different impacts. A feature that impacts team leads may not impact engineers.

### Level 3: Impacts (How?)

**How should each actor's behavior change to achieve the goal?**

This is the **outcome** level—the behavior or mindset shift you're aiming for. Impacts are **not features**. Examples:
- Team leads **invite more teammates** after initial setup
- DevOps engineers **configure alerts in <5 minutes** instead of abandoning
- Executives **renew annual contracts** based on demonstrated ROI

**Impacts answer**: "If we succeed, what will actors **do differently**?"

### Level 4: Deliverables (What?)

**What can we do (features, experiments, changes) to support the desired impacts?**

**Only now** do you define features. And crucially, **features are hypotheses**—you believe Feature X will cause Impact Y for Actor Z, helping achieve Goal W.

**Example deliverable**:
- **Deliverable**: Onboarding wizard with team invite prompt
- **Supports Impact**: Team leads invite more teammates
- **For Actor**: Team leads
- **To Achieve Goal**: Increase Monthly Active Teams by 25%

If the deliverable **doesn't** change the actor's behavior (impact), it doesn't contribute to the goal. **Kill it or pivot.**

---

## The Builder's Hierarchy in Practice

CloudOps adopted Impact Mapping, creating a **strategic hierarchy** for Q4:

| **Level** | **Example** | **Owner** | **Decision Authority** |
|-----------|-------------|-----------|------------------------|
| **Goal** | Increase Monthly Active Teams by 25% in Q4 | CEO / Leadership | Approve/change strategic goals |
| **Actors** | Team leads, DevOps engineers | Product Leadership | Prioritize which actors to focus on |
| **Impacts** | Team leads invite 3+ teammates within first week | Product Managers | Define target behaviors per actor |
| **Deliverables** | Onboarding wizard with invite prompt | Squad/Team | Choose specific features/solutions |

### Traceability in Action

When a feature request came in ("Add Slack integration"), Rachel asked the **hierarchy questions**:

1. **Which goal does this serve?** "Increase Monthly Active Teams"
2. **Which actor benefits?** "Team leads"
3. **What impact do we expect?** "Team leads notify teammates via Slack, increasing activation"
4. **Is this the best deliverable for that impact?** "Maybe. Let's validate: Do team leads already use Slack? Would in-app notifications work as well?"

**Outcome**: They validated that 78% of team leads used Slack. They built the integration, measured impact (team invites increased by 19%), and **contributed measurably to the goal**.

**Contrast**: Another request ("Add dark mode") couldn't trace to any goal or impact. **Killed**—not because dark mode is bad, but because it didn't align with Q4 strategy.

---

## TOGAF Capability Mapping: Enterprise-Scale Hierarchy

For larger organizations, **TOGAF (The Open Group Architecture Framework)** provides **Capability-Based Planning**—a strategic approach that maps business capabilities to IT investments (5, 6).

### What Are Business Capabilities?

**"The business capability map provides a self-contained view of the business that is independent of the current organizational structure, business processes, IT systems and applications, and the product or service portfolio"** (7).

**Key insight**: Capabilities are **what the business does**, independent of **how** it's currently organized or **what tools** it uses. Examples:
- **Customer Onboarding** (capability) exists whether you have 1 team or 10, whether you use Salesforce or HubSpot
- **Incident Response** (capability) exists whether engineers handle it manually or via automation

### Capability Mapping Benefits

**TOGAF maps business capabilities back to** (6, 7):
1. **Organizational units**: Which teams own which capabilities?
2. **Value streams**: How do capabilities connect to deliver customer value?
3. **Information systems**: Which IT systems support which capabilities?
4. **Strategic plans**: Which capabilities need investment to achieve strategy?

This provides **greater insight into alignment and optimization** (6).

### Capability-Based Planning Process

**"Capability management is aligned with Enterprise Architecture, with all architectures expressed in terms of business outcomes and value rather than in IT terms"** (8).

The process:
1. **Corporate Strategy** drives Architecture Vision (TOGAF Phase A)
2. **Capabilities** are identified and mapped to strategic goals
3. **Capability Gaps** are identified (current state vs. desired state)
4. **Projects/Portfolios** are created to close capability gaps
5. **Architecture Definition** (Phases B-D) specifies how to build/enhance capabilities
6. **Phase E Projects** deliver incremental capability improvements

**"Capability managers perform similar tasks to portfolio managers, but across the portfolios aligning the projects and project increments to deliver continuous business value"** (8).

---

## Hierarchy Levels and Decision Authority

A key principle of Builder's Hierarchy: **Different levels require different decision-making authority**. Clarity prevents bottlenecks and empowers teams.

### The Four-Level Model (Synthesizing Impact Mapping + TOGAF)

| **Level** | **Description** | **Horizon** | **Decision Owner** | **Key Question** |
|-----------|-----------------|-------------|-------------------|------------------|
| **1. Outcomes** | Strategic business goals | Quarters/Years | Leadership / Executives | Why does this matter to the business? |
| **2. Capabilities** | What the business must do to achieve outcomes | Quarters | Product Leadership / Capability Owners | What capabilities enable this outcome? |
| **3. Features** | Specific product functionality | Months | Product Managers / Squad Leads | Which features deliver this capability? |
| **4. Tasks** | Implementation work | Weeks/Sprints | Engineers / Designers | How do we build this feature? |

### Decision Rights Per Level

**Level 1 (Outcomes)**:
- **Who decides**: CEO, Leadership Team, Board
- **Decisions**: Strategic priorities, resource allocation across outcomes, when to pivot
- **Frequency**: Quarterly (with annual strategy refresh)

**Level 2 (Capabilities)**:
- **Who decides**: VP Product, Capability Owners, Portfolio Managers
- **Decisions**: Which capabilities to invest in, capability roadmaps, cross-team coordination
- **Frequency**: Monthly/Quarterly

**Level 3 (Features)**:
- **Who decides**: Product Managers, Squad Leads
- **Decisions**: Feature prioritization, scope, success metrics, when to kill features
- **Frequency**: Bi-weekly/Sprint Planning

**Level 4 (Tasks)**:
- **Who decides**: Engineers, Designers, individual contributors
- **Decisions**: Implementation approach, technical design, task breakdown
- **Frequency**: Daily/Sprint

### Why This Matters

**Without clear decision rights**:
- Every decision escalates to leadership → **bottleneck**
- Teams feel disempowered → **morale suffers**
- Strategic decisions get bogged down in implementation details → **slow execution**

**With clear decision rights**:
- Teams make decisions **at the appropriate level**
- Leadership focuses on outcomes, not features
- Execution velocity increases

---

## Preventing Strategic Drift: Alignment Mechanisms

Even with a hierarchy, drift happens unless there are **active alignment mechanisms**.

### Mechanism 1: Mandatory Traceability

**Every feature must trace to a capability, which traces to an outcome.**

**Implementation**:
- **Tool enforcement**: JIRA/Linear configured so every story requires a "Strategic Objective" tag
- **Planning review**: During sprint planning, PM must articulate the traceability path for each feature
- **Killswitch**: If traceability is unclear, feature is **blocked** until clarified or killed

### Mechanism 2: Quarterly Capability Review

**Assess capability health and alignment.**

**Process**:
1. **Capability owners** present:
   - Current capability maturity (e.g., "Onboarding" is 60% mature)
   - Contribution to strategic outcomes (e.g., "Onboarding improved activation by 12%, contributing to 25% MAU goal")
   - Gaps and investment needs
2. **Leadership decides**: Continue investment, reduce investment, or kill capability

### Mechanism 3: Outcome-Based Retrospectives

**Traditional retro**: "What went well? What didn't? What can we improve?"

**Outcome-based retro**: "Did we move the outcome metric? If not, why? What hypothesis was wrong?"

**Example**:
- **Goal**: Increase Monthly Active Teams by 25%
- **Actual**: Increased by 8%
- **Retro question**: "We shipped 12 features this quarter. Which ones moved the metric? Which didn't? Why?"
- **Learning**: 3 features drove the 8% increase; 9 features had zero impact → **kill or pivot those 9**

### Mechanism 4: Decision Journals (Per Level)

Inspired by **Architecture Decision Records (ADRs)**, maintain decision journals at each level:

- **Outcome Decision Record**: Why we chose this strategic goal, what we're betting on, success criteria
- **Capability Decision Record**: Why we're investing in this capability, alternatives considered, expected impact
- **Feature Decision Record**: Why we built this feature, which impact it supports, how we'll measure success

**Benefit**: When drift occurs, you can trace back to **where the decision diverged from strategy**.

---

## Case Study: TechServe's Hierarchy Transformation

**Context**:
TechServe, a B2B SaaS platform with 150 engineers across 12 teams, had a **strategic alignment crisis**. Annual revenue grew 15% (target was 40%). Customer churn was 7% (target was 3%). The product roadmap had 200+ features in the backlog, but **no one could explain how features connected to revenue or churn**.

**Before Builder's Hierarchy**:
- **Backlog**: 200+ feature requests from sales, support, customers, executives
- **Prioritization**: Political—loudest voice wins
- **Traceability**: None—teams couldn't answer "Why are we building this?"
- **Decision authority**: Everything escalated to CPO; teams waited days for answers
- **Strategic alignment**: 0%—features had no connection to revenue or churn goals

**Problems**:
- **Feature factory** (Chapter 3): Teams measured success by features shipped, not outcomes
- **80% feature waste**: Post-launch analysis showed 79% of features had <5% adoption
- **Strategic paralysis**: Leadership debating every feature request; roadmap unchanged for 6 months

**Metrics (Before)**:
- **Strategic alignment score**: 22% (team survey: "I understand how my work connects to company goals")
- **Feature-to-outcome traceability**: 0% (no features traced to strategic goals)
- **Decision cycle time**: 8.4 days (median time from feature idea to go/no-go decision)
- **Unused features**: 79% (<5% adoption 90 days post-launch)
- **Team autonomy score**: 31% ("I can make decisions without escalation")

**Transformation**:
TechServe implemented Builder's Hierarchy using Impact Mapping + TOGAF principles:

1. **Defined Outcomes** (Leadership workshop):
   - **Outcome 1**: Increase Annual Recurring Revenue (ARR) by 40% → $50M
   - **Outcome 2**: Reduce churn from 7% to 3%
   - **Outcome 3**: Expand into enterprise segment (>1,000 employee companies)

2. **Identified Capabilities** (Product Leadership):
   - For **Outcome 1** (Revenue): Sales Enablement, Customer Onboarding, Product-Led Growth
   - For **Outcome 2** (Churn): Customer Success, Product Reliability, Feature Adoption
   - For **Outcome 3** (Enterprise): Enterprise Security, Admin Controls, Integration Ecosystem

3. **Mapped Actors & Impacts** (Product Managers):
   - **Actor**: Sales reps → **Impact**: Close deals 20% faster using product demos
   - **Actor**: New customers → **Impact**: Activate within 48 hours (vs. 7 days)
   - **Actor**: At-risk customers → **Impact**: Engage with success manager before churning

4. **Prioritized Deliverables** (Squads):
   - **Top 20 features** traced to Actors/Impacts/Outcomes
   - **180 features killed** (couldn't trace to any outcome)
   - Each squad owned 1-2 capabilities; full autonomy within capability boundaries

5. **Enforced Traceability**:
   - JIRA configured: Every story requires "Outcome" and "Capability" tags
   - Sprint planning template: "Which outcome does this serve? Which actor? What impact?"
   - Quarterly reviews: Capability owners present outcome contributions

6. **Clear Decision Authority**:
   - **Outcomes**: CEO (quarterly)
   - **Capabilities**: CPO (monthly review)
   - **Features**: Product Managers (sprint planning)
   - **Tasks**: Engineers (daily)

**After Builder's Hierarchy**:
- **Strategic alignment score**: 22% → **81%** (269% improvement)
- **Feature-to-outcome traceability**: 0% → **100%** (enforced in JIRA)
- **Decision cycle time**: 8.4 days → **1.2 days** (86% reduction; decisions made at right level)
- **Unused features**: 79% → **18%** (77% reduction; killed 180 features pre-build)
- **Team autonomy score**: 31% → **74%** (teams empowered within capability boundaries)

**Business Outcomes**:
- **ARR growth**: Increased from 15% to **38%** (close to 40% target)
- **Churn**: Reduced from 7% to **3.4%** (on track to 3%)
- **Enterprise expansion**: Landed 6 enterprise deals (>1,000 employees)

**Cultural Shifts**:
- **"Ship features" → "Move outcomes"**: Teams celebrated outcome improvements, not feature counts
- **"Everything is important" → "Strategic clarity"**: 180 features killed without drama; everyone understood why
- **"Escalate decisions" → "Own decisions"**: Teams made 85% of decisions autonomously within capability boundaries
- **"Build what's requested" → "Validate before building"**: Every feature had success criteria tied to impact

**Key Learning**:
**Hierarchy isn't bureaucracy**—it's **clarity**. When every person understands the outcome they're serving, the capability they're building, and the impact they're targeting, **autonomy and alignment coexist**. TechServe's velocity **increased** (more decisions made faster) while strategic alignment **improved** (decisions connected to outcomes).

---

## Anti-Patterns: Where Hierarchy Breaks Down

### 1. **Feature Backlog Without Outcome Traceability**
**Pattern**: Backlog full of feature requests with no link to business goals.
**Problem**: Teams can't answer "why are we building this?" beyond "stakeholder asked for it."
**Correction**: **Impact Mapping**—every feature traces to actor impact and business goal (1, 3).

### 2. **Too Many Hierarchy Levels**
**Pattern**: 7+ levels (Outcomes → Themes → Epics → Capabilities → Features → Stories → Tasks → Subtasks).
**Problem**: Decision paralysis, unclear authority, bureaucracy (Chapter 15).
**Correction**: **3-4 levels maximum** (Outcomes → Capabilities → Features → Tasks).

### 3. **Bottom-Up Hierarchy**
**Pattern**: Define tasks/features first, retrofit into capabilities/outcomes later.
**Problem**: Strategic incoherence; features don't align when rolled up.
**Correction**: **Top-down**—start with outcome, decompose to capabilities, then features.

### 4. **Capability Mapping Without Refresh**
**Pattern**: Create capability map once, never update as business evolves.
**Problem**: Capabilities misaligned with current strategy; map becomes shelf-ware.
**Correction**: **Quarterly capability review** aligned with strategic planning cycles (5, 8).

### 5. **No Decision Rights Per Level**
**Pattern**: Unclear who decides at each hierarchy level.
**Problem**: Every decision escalates; bottlenecks at leadership.
**Correction**: **Clear decision authority**—outcomes (exec), capabilities (product), features (squad), tasks (eng).

### 6. **Hierarchy Without Traceability Tools**
**Pattern**: Hierarchy exists conceptually but not enforced in tools.
**Problem**: Alignment invisible; can't prove strategic progress.
**Correction**: **Tool configuration** enforcing hierarchy (epics → stories with mandatory strategic tag).

### 7. **Autonomy Without Alignment (Spotify Lesson)**
**Pattern**: Autonomous squads empowered to make decisions without clear hierarchy.
**Problem**: Squads building features misaligned with company objectives (9).
**Correction**: **Autonomy requires hierarchical clarity**—squads need to understand where their work fits in the hierarchy.

---

## Reflection Questions

1. **Traceability Test**: Pick three features in your current roadmap. Can you trace each to an outcome, actor, and impact? If not, should they be in the roadmap?

2. **Backlog Audit**: What percentage of your backlog has **clear traceability** to strategic goals? What happens to features that don't trace?

3. **Decision Authority**: For the last 10 product decisions, who made them? Were they at the appropriate hierarchy level, or did they escalate unnecessarily?

4. **Capability Clarity**: Can you name your product's **core capabilities**? Do teams understand which capability they own?

5. **Outcome Visibility**: Can every team member articulate the **top 3 strategic outcomes** for this quarter? If not, how will they make aligned decisions?

6. **Kill Discipline**: When was the last time you **killed a feature pre-build** because it didn't trace to an outcome? If "never," why not?

---

## Summary: Hierarchy as Strategic Clarity, Not Bureaucracy

The **Builder's Hierarchy** isn't about adding process—it's about **adding clarity**. When outcomes, capabilities, features, and tasks form an explicit, traceable hierarchy, **strategic alignment becomes visible and actionable**.

**Key insights from this chapter**:

1. **Strategic drift is the default**: Without explicit hierarchy, **features become shopping lists**, disconnected from business goals. **"Even though the features are delivered, often the business objective is not achieved"** (Gojko Adzic) (1).

2. **Impact Mapping provides a 4-level hierarchy**: **Goal → Actors → Impacts → Deliverables**. Every deliverable traces to an impact for an actor to achieve a goal (3, 4).

3. **TOGAF Capability-Based Planning scales hierarchy to enterprises**: Business capabilities are **independent of org structure, tools, and processes**—they represent **what the business does** (7). Mapping capabilities to strategic plans enables portfolio coordination (6, 8).

4. **Decision authority per level prevents bottlenecks**: Outcomes (leadership), Capabilities (product), Features (squads), Tasks (engineers). Clear rights empower teams and focus leadership on strategy.

5. **Traceability mechanisms prevent drift**: Mandatory feature-to-outcome tracing, quarterly capability reviews, outcome-based retrospectives, and decision journals keep alignment active.

6. **Autonomy requires alignment**: The Spotify lesson—**autonomous teams without hierarchical clarity drift into misalignment** (9). Hierarchy provides the **boundaries** within which autonomy thrives.

7. **Killing features is strategic discipline**: TechServe killed **180 of 200 features** because they didn't trace to outcomes. This **freed capacity** for the 20 features that mattered, reducing unused features from 79% to 18%.

The **Builder's Hierarchy** transforms backlogs from "everything stakeholders want" into "only what serves strategic outcomes." It's not about saying "yes" to everything—it's about knowing **why you're saying no**.

In the next chapter, we explore **Cognitive Load Engineering**—the discipline of designing products and codebases that respect human cognitive limits, ensuring systems remain comprehensible as they grow.

---

## References

1. Adzic, G. (n.d.). *Impact Mapping*. Retrieved from https://gojko.net/books/impact-mapping/

2. EBG Consulting. (n.d.). *Software That Matters: A Review of Gojko Adzic's Impact Mapping*. Retrieved from https://www.ebgconsulting.com/blog/software-that-matters-a-review-of-gojko-adzics-impact-mapping/

3. Open Practice Library. (n.d.). *Impact Mapping*. Retrieved from https://openpracticelibrary.com/practice/impact-mapping/

4. Impact Mapping. (n.d.). *Impact Mapping: Making a Big Impact*. Retrieved from https://www.impactmapping.org/

5. KnowledgeHut. (n.d.). *TOGAF Business Capability Model: Definitive Guide*. Retrieved from https://www.knowledgehut.com/blog/it-service-management/business-capability-modelling

6. The Open Group. (n.d.). *The TOGAF Standard - Business Capabilities*. Retrieved from https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html

7. The Open Group. (n.d.). *TOGAF Business Capability*. Retrieved from https://pubs.opengroup.org/togaf-standard/business-architecture/business-capabilities.html

8. The Open Group. (n.d.). *The TOGAF Standard - Capability-Based Planning*. Retrieved from https://pubs.opengroup.org/architecture/togaf9-doc/arch/chap28.html

9. Common industry knowledge: Spotify model evolution and lessons on autonomy vs. alignment

---

**Word Count**: ~4,900
