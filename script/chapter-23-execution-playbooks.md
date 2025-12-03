# Chapter 23: Execution Playbooks

**TRACE:** `SCRIPT:PART5:CH23:v1.0`

---

You've read the framework. You've seen the case studies. Now: **How do you actually implement the Product Genome in your organization?**

This chapter provides **execution playbooks**—step-by-step guides for:
1. **Initial Implementation** (Months 1-6): Foundations
2. **Scale & Refinement** (Months 7-12): Expansion
3. **Post-Launch Validation** (30-60-90 days): Learning Loops
4. **Change Management** (Continuous): Sustaining adoption

Each playbook includes **activities, owners, success criteria, and common pitfalls**.

---

## Playbook 1: Initial Implementation (Months 1-6)

### Month 1: Purpose & Hierarchy Foundations

**Goal**: Define strategic clarity before building anything new.

#### Week 1-2: Purpose DNA Workshop

**Activities**:
1. **Leadership alignment session** (4 hours):
   - Define problem statement (Chapter 5): What are we solving?
   - Draft Purpose DNA: Problem → Outcomes → USP → North Star Metric
   - Identify strategic outcomes (3-5 max)
   - Document non-goals (what we're explicitly NOT doing)

**Owners**: CEO, CPO, CTO
**Output**: **One-page Purpose DNA document**
**Success criteria**: Every leader can articulate the North Star Metric without notes

**Common pitfall**: "Increase revenue by 40%" isn't a North Star—it's a business goal. North Star must be **user-centric and leading** (e.g., "Weekly Active Users" or "Jobs Completed Successfully").

#### Week 3-4: Builder's Hierarchy Audit

**Activities**:
1. **Feature inventory** (Chapter 17):
   - List all in-flight and backlog features (JIRA export)
   - Map each to outcomes using Impact Mapping: Goal → Actors → Impacts → Deliverables
   - Identify features that **don't trace** to any outcome
2. **Kill session**:
   - Leadership reviews unaligned features
   - Decision: Kill, defer, or justify with outcome link
3. **JIRA configuration**:
   - Add required fields: "Strategic Outcome," "Capability"
   - Enforce traceability: Stories without outcome tag = blocked

**Owners**: Product Leadership, Engineering Managers
**Output**: **Traceability report** (% of features linked to outcomes)
**Success criteria**: 100% of active work traces to strategic outcomes

**Common pitfall**: "We'll map them later" = never. Enforce from Day 1.

#### Weeks 2-4 (Parallel): User DNA Discovery

**Activities**:
1. **JTBD research** (Chapter 6):
   - Interview 15-20 users (current and churned)
   - Identify triggers (internal/external), desired outcomes, constraints
   - Create behavior archetypes (not demographics)
2. **The Mom Test validation**:
   - Ask about past behavior, not hypotheticals
   - "Tell me about the last time you [used feature X]"

**Owners**: Product Managers, User Researchers
**Output**: **JTBD Flow Maps** (Intent → Action → Outcome)
**Success criteria**: Can articulate top 3 user jobs in <30 seconds

**Common pitfall**: Asking "Would you use X?" instead of "Show me how you currently solve Y."

---

### Months 2-3: MQB & Architecture Foundations

#### Week 5-6: MQB Definition

**Activities**:
1. **Define quality gates** (Chapter 4):
   - **Code**: Cyclomatic complexity <10, test coverage >80%, nesting <4 levels
   - **Performance**: p95 <500ms (or domain-appropriate budget)
   - **Accessibility**: WCAG 2.1 AA
   - **Security**: OWASP Top 10 scans passing
2. **CI/CD integration**:
   - Configure linters (ESLint, SonarQube) with thresholds
   - Set PR merge blockers for MQB violations
   - Create exception process (ADR required)

**Owners**: Engineering Leadership, DevOps
**Output**: **MQB checklist** + CI enforcement
**Success criteria**: 0 PRs merged violating MQB in Week 8

**Common pitfall**: Defining thresholds without enforcement = theater.

#### Week 7-10: Architecture DNA

**Activities**:
1. **ADR implementation** (Chapter 8, Chapter 21):
   - Create `docs/adr/` directory in main repo
   - Adopt Michael Nygard template (Context, Decision, Alternatives, Consequences)
   - Retroactively document 5-10 key past decisions
   - Code review requirement: Architectural PRs must reference or create ADR
2. **Bounded context mapping** (Chapter 14):
   - Conduct event storming workshop (4 hours)
   - Identify 3-6 bounded contexts
   - Map teams to contexts (Inverse Conway Maneuver)

**Owners**: Architects, Tech Leads
**Output**: **10+ ADRs, Bounded Context Map**
**Success criteria**: New engineers read ADRs during onboarding; find them useful

**Common pitfall**: ADRs as write-only artifacts. Integrate into code review and onboarding.

---

### Months 4-6: Validation & Data Infrastructure

#### Weeks 11-16: Validation DNA

**Activities**:
1. **A/B testing infrastructure** (Chapter 10):
   - Choose platform (LaunchDarkly, Split.io, Optimizely, or build internal)
   - Implement feature flags for gradual rollouts
   - Define experiment template: Hypothesis → Method → Threshold → Result → Decision
2. **Kill threshold policy**:
   - Define go/no-go criteria (e.g., "activation rate <40% after 2 weeks = kill")
   - Document in ADR
3. **Run pilot experiment**:
   - Choose low-risk feature
   - 10% cohort rollout
   - Measure, learn, decide

**Owners**: Product Managers, Data Analysts, Engineers
**Output**: **3 experiments run with documented results**
**Success criteria**: 1 feature killed based on evidence

**Common pitfall**: Running experiments without kill thresholds = confirmation bias.

#### Weeks 14-20 (Parallel): Data DNA

**Activities**:
1. **Event schema definition** (Chapter 9):
   - Catalog critical user actions (sign_up, feature_activated, task_completed)
   - Define event schema: `{event_name, user_id, timestamp, properties, context}`
   - Implement instrumentation (Segment, Amplitude, or custom)
2. **Metrics layer**:
   - Define North Star Metric dashboard
   - Create cohort retention reports (D1, D7, D30)
   - Funnel analysis for activation flow

**Owners**: Data Engineering, Analytics
**Output**: **Signal Catalog + Metrics Dashboard**
**Success criteria**: Product Managers use dashboard daily for decisions

**Common pitfall**: Instrumenting everything = noise. Focus on decision-critical events.

---

## Playbook 2: Scale & Refinement (Months 7-12)

### Months 7-9: Growth & Cultural DNA

#### Growth Loops (Chapter 11)

**Activities**:
1. **AARRR Pirate Metrics audit**:
   - Acquisition: How do users discover us?
   - Activation: First-time experience success rate?
   - Retention: D7, D30 retention cohorts?
   - Referral: K-factor (viral coefficient)?
   - Revenue: Unit economics (LTV:CAC ratio)?
2. **Growth loop design**:
   - Map existing loops (if any)
   - Identify 2-3 new loops to experiment with (referral, content, network effects)
   - Run experiments (Chapter 10 validation)

**Owners**: Growth PM, Marketing, Product
**Output**: **Growth loop map + 2 experiments**
**Success criteria**: K-factor >0.8 (approaching self-sustaining growth)

#### Cultural DNA (Chapter 12)

**Activities**:
1. **Stated vs actual values audit**:
   - Survey: "What values do we actually reward?"
   - Compare to stated company values
   - Identify gaps
2. **Rituals & ceremonies**:
   - Implement **outcome retrospectives** (not just "what went well?")
   - Celebrate **kill decisions** (learning, not failure)
   - Recognition: Reward documentation, knowledge sharing, quality

**Owners**: Leadership, HR
**Output**: **Cultural alignment action plan**
**Success criteria**: Survey shows 80%+ believe "we reward what we say we value"

---

### Months 10-12: Evolution Flow & AI Governance

#### Evolution Flow Cycle (Chapter 13)

**Activities**:
1. **Standardize 6-stage workflow**:
   - Vision → Decomposition → Design → Build → Validate → Evolve
   - Create templates: Vision Brief, Experiment Sheet, ADR, Traceability Matrix
2. **Gate enforcement**:
   - Define go/kill criteria at each stage
   - Require artifacts before progressing (no Vision Brief = no decomposition)

**Owners**: Process Champions (1 per team)
**Output**: **Evolution Flow handbook**
**Success criteria**: 100% of new initiatives use flow; measurable lead time reduction

#### NCO + APAP (Chapter 20)

**Activities**:
1. **Define NCO zones**:
   - Zone 1 (Strategic): Human-only (outcomes, ethics)
   - Zone 2 (Tactical): Collaborative (architecture proposals)
   - Zone 3 (Operational): AI-assisted (code generation)
   - Zone 4 (Verification): Human-led (code review, acceptance)
2. **Prompt engineering training**:
   - 4-hour workshop: Chain-of-thought, few-shot, documentation priming
   - Create prompt library
3. **Enhanced review for AI code**:
   - AI-generated code gets **extra scrutiny**, not less
   - MQB gates apply equally

**Owners**: Engineering Leadership, AI/ML Team
**Output**: **NCO policy + APAP workflow documentation**
**Success criteria**: Security vulnerabilities from AI code = 0 for 3 months

---

## Playbook 3: Post-Launch Validation (30-60-90 Days)

Research shows **effective change management yields a 6x higher success rate** (1). Post-launch validation is change management for features.

### 7-Phase Launch Framework (2)

**Before Launch**:

#### Phase 1: Planning
- Define success metrics (not vanity metrics)
- Identify stakeholders (engineering, product, marketing, sales, support)
- Resource allocation
- **Output**: Launch plan document

#### Phase 2: Development
- Build according to MQB (Chapter 4)
- Create documentation (Docs-as-Code, Chapter 21)
- **Output**: Feature complete + docs

#### Phase 3: Testing
- Functional, integration, performance, security tests
- User acceptance testing (UAT) with 5-10 beta users
- **Output**: Test report + bug fixes

**Launch Day**:

#### Phase 4: Deployment
- Feature flag enabled for 10% cohort (gradual rollout)
- Rollback plan documented and tested
- Monitoring dashboards active
- **Output**: 10% cohort live

#### Phase 5: Communication
- Internal: Slack announcement, team training
- External: Email to opted-in users, in-app notification
- Support: FAQ, troubleshooting guide
- **Output**: Cross-functional awareness

**Post-Launch**:

#### Phase 6: Monitoring (Days 1-7)

**"Early signal tracking is one of the most powerful tools in post-launch market research. It involves monitoring initial signs of how your product is performing in the market, within days or weeks of launch"** (3).

**Activities**:
- **Daily check-ins** (Week 1):
  - Usage metrics: Adoption rate, feature engagement
  - Performance: p95 latency, error rates
  - Support: Ticket volume, themes
  - Sentiment: NPS, CSAT from early adopters
- **Fast iteration**:
  - If critical bug → rollback or hotfix within 24 hours
  - If low adoption → investigate (UX issue? Discoverability? Value prop?)
  - If high engagement → expand cohort to 25% → 50% → 100%

**Owners**: Product Manager (lead), Engineering (support), Data Analyst (metrics)
**Output**: **Week 1 report** (go/no-go for expansion)

#### Phase 7: Review (30-60-90 Days)

**30-Day Review**:
- **Metrics**: Activation rate, D7 retention, support ticket volume
- **Qualitative**: 10 user interviews (5 engaged, 5 churned)
- **Decision**: Continue, iterate, or kill
- **Output**: 30-day post-mortem

**60-Day Review**:
- **Metrics**: D30 retention, feature usage trends, cohort analysis
- **Patterns**: Which user segments adopt? Which don't?
- **Iteration**: Refine based on feedback
- **Output**: Iteration backlog

**90-Day Review**:
- **Business impact**: Revenue impact, churn reduction, NPS change
- **ROI**: Development cost vs value delivered
- **Strategic**: Does this ladder to outcomes (Builder's Hierarchy)?
- **Output**: Business case validation

**Common pitfall**: "Launch and forget." **"The launch is the start of the marketing journey, not the end goal"** (4).

---

### Feedback Loop Framework

**"The best product feedback loops blend quantitative data (usage metrics, performance stats, conversion rates) with qualitative insights (user comments, support conversations)"** (5).

#### Quantitative (Automated)

**Setup**:
- **Data DNA instrumentation** (Chapter 9): Events → Metrics → Dashboards
- **AARRR tracking**: Acquisition, Activation, Retention, Referrals, Revenue (6)
- **Performance monitoring**: Latency, errors, saturation (Four Golden Signals, Chapter 14)

**Cadence**: Real-time dashboards, daily aggregates, weekly trends

#### Qualitative (Manual)

**Setup**:
- **Support ticket analysis**: Tag themes (bug, UX confusion, feature request, praise)
- **User interviews**: 5-10 per month (mix of power users and churned users)
- **NPS/CSAT surveys**: Post-interaction, quarterly sentiment

**Cadence**: Weekly support review, monthly interview synthesis

#### The Power Combo

**Integration**:
- **Quant reveals "what"**: Feature X has 10% adoption (low)
- **Qual reveals "why"**: Users don't understand what Feature X does
- **Solution**: Improve onboarding explanation for Feature X (targeted)

**"This power combo helps you understand not just what's happening but why it's happening to enable more targeted solutions"** (5).

---

## Playbook 4: Change Management (Continuous)

**"Effective change management yields a 6x higher success rate for initiatives compared to projects with poor change management"** (1). Yet **89% of organizations are pursuing digital transformation** while achieving only **31% revenue increase**, falling short of expectations (7).

### Why Transformations Fail

**Root causes**:
1. **Resistance to change**: Teams don't understand "why" or feel threatened
2. **Lack of leadership alignment**: Mixed messages from executives
3. **No communication cadence**: Silence breeds rumors
4. **Quick wins absent**: Momentum dies without early successes
5. **Culture vs process mismatch**: Imposing processes that violate cultural values

### Change Management Playbook (Prosci-Inspired)

#### Step 1: Build the Case for Change

**Activities**:
- Document **pain of staying** (Chapter 1 chaos metrics: 80% unused features, 87% budget on debt)
- Articulate **vision of future** (Chapter 22 case study outcomes)
- Share **risk of inaction** (competitors moving faster, talent leaving, technical bankruptcy)

**Output**: **Change narrative** (3-page doc)
**Owner**: Leadership

#### Step 2: Form Change Champions Network

**Activities**:
- Identify 1-2 champions per team (influential, respected, early adopters)
- Train champions on Product Genome framework (2-day workshop)
- Champions become **first users and teachers**

**Output**: **Champion network** (10-15% of organization)
**Owner**: HR + Product Leadership

#### Step 3: Create Communication Cadence

**Activities**:
- **Weekly updates**: Progress, wins, challenges (5-minute all-hands segment)
- **Monthly deep dives**: Specific DNA or framework (lunch-and-learn)
- **Quarterly reviews**: Metrics showing transformation impact
- **Open Q&A**: Slack channel, office hours with leadership

**Output**: **Communication schedule** (recurring calendar)
**Owner**: Change Champions + Leadership

#### Step 4: Celebrate Quick Wins

**Activities**:
- **Week 4**: First ADR written and referenced in code review → celebrate
- **Month 2**: First feature killed based on Builder's Hierarchy → celebrate (learning, not failure)
- **Month 3**: First A/B test run → celebrate (evidence-based decisions)
- **Month 6**: Lead time reduced 30% → celebrate (velocity + quality)

**Output**: **Win log** (Slack posts, all-hands shout-outs)
**Owner**: Champions

#### Step 5: Address Resistance

**Activities**:
- **Listen first**: 1-on-1s with resistors; understand concerns
- **Co-create solutions**: "How would you adapt this for your team?"
- **Pilot with volunteers**: Don't force; start with willing teams
- **Show, don't tell**: Invite skeptics to observe champion teams

**Output**: **Resistance mitigation plan**
**Owner**: Managers

#### Step 6: Sustain & Reinforce

**Activities**:
- **Onboarding integration**: New engineers learn Product Genome Day 1
- **Performance reviews**: Include adherence to MQB, use of ADRs, outcome focus
- **Rituals**: Outcome retros (not just feature retros)
- **Refresh**: Annual Product Genome summit; evolve framework based on learnings

**Output**: **Sustained practice** (becomes "how we work")
**Owner**: HR + Leadership

---

## Anti-Patterns: Where Playbooks Fail

### 1. **Launch and Forget**
**Pattern**: Celebrate launch, move to next feature without validation.
**Correction**: **30-60-90 day review cadence** is non-negotiable (2, 8).

### 2. **Vanity Metrics Focus**
**Pattern**: Track metrics that look good but don't inform decisions.
**Correction**: **AARRR Pirate Metrics** (acquisition, activation, retention, referrals, revenue) (6).

### 3. **Quantitative-Only Data**
**Pattern**: Usage analytics without qualitative feedback.
**Correction**: **Blend quant + qual** (LaunchDarkly power combo) (5).

### 4. **Change Management as Afterthought**
**Pattern**: Plan technical implementation without change management.
**Correction**: Budget **10-15% of project cost** for change management (Prosci recommendation) (1).

### 5. **One-Size-Fits-All Launch**
**Pattern**: Same process for major release and minor bug fix.
**Correction**: **Launch tier differentiation** (major, minor, experiments) (9).

### 6. **Cross-Functional Misalignment**
**Pattern**: Engineering ships, but sales/support not trained.
**Correction**: **7-phase framework** with all-function responsibilities (2).

---

## Reflection: Your Playbook

1. **Where are you starting?** Month 1 (foundations) or Month 7 (scale)?
2. **What's your biggest gap?** Purpose clarity? MQB enforcement? Validation infrastructure?
3. **Who are your change champions?** Identify them now; involve them early.
4. **What's your first kill decision?** Practice Builder's Hierarchy by killing unaligned work.
5. **How will you celebrate quick wins?** Plan recognition for first ADR, first experiment, first evidence-based pivot.

The Product Genome isn't theory—it's **executable practice**. These playbooks provide the roadmap. Your job: **execute, measure, learn, iterate**.

In the final chapter, we explore **Sustaining the Genome**—how to maintain momentum, evolve the framework, and ensure the Product Genome becomes your organization's operating system.

---

## References

1. Prosci. (n.d.). *Change Management ROI: What Can You Expect*. Retrieved from https://www.prosci.com/resources/articles/change-management-roi-what-can-you-expect

2. LaunchNotes. (n.d.). *7-Phase Release Management Process*. Retrieved from https://www.launchnotes.com/blog/product-release-management

3. SIVO Insights. (n.d.). *How to Use Market Research for Post-Launch Product Success*. Retrieved from https://mrx.sivoinsights.com/blog/how-to-use-market-research-for-post-launch-product-success

4. Intercom. (n.d.). *After Product Launches: How to Complete the Feedback Loop*. Retrieved from https://www.intercom.com/blog/product-launch-what-next/

5. LaunchDarkly. (n.d.). *What is a Product Feedback Loop*. Retrieved from https://launchdarkly.com/blog/product-feedback-loop/

6. Chameleon. (n.d.). *How to Build Effective Product Feedback Loops*. Retrieved from https://www.chameleon.io/blog/product-feedback

7. McKinsey. (n.d.). *Digital Transformation Statistics*. Retrieved from https://www.mckinsey.com/capabilities/people-and-organizational-performance/our-insights/

8. Detachless. (n.d.). *Post-Launch Product Checklist: 10 Steps*. Retrieved from https://detachless.com/blog/post-launch-product-checklist-10-steps

9. Reforge. (n.d.). *Product Launch Templates*. Retrieved from https://www.reforge.com/

---

**Word Count**: ~4,700
