# Chapter 6: User DNA — Reality Anchor

**TRACE:** `SCRIPT:PART2:CH06:v1.0`
**Word Count Target:** 5,500–6,000 words
**Status:** Draft v1.0

---

## Opening: The Imaginary User Problem

Three years ago, I sat in on a product demo where a team proudly showed off six months of work: a sophisticated analytics dashboard with 47 different chart types, customizable filters, and AI-powered insights.

"This is amazing," the VP of Product said. "Our users are going to love this."

I asked a simple question: "Which users? What job are they hiring this to do?"

Silence.

Eventually, someone said, "Well, data analysts will use it to... analyze data."

Another added, "And executives can get insights faster."

A third suggested, "Anyone who needs to understand their metrics."

Every answer was technically true. None of them was specific enough to guide a single design decision.

They had built a product for imaginary users—generic personas conjured from assumptions rather than evidence. "Data analysts" who might or might not exist in their customer base. "Executives" with unspecified needs in undefined contexts. "Anyone" who needs "insights" for unspecified purposes.

Six months later, usage data told the story: **8% of customers had opened the dashboard. 2% used it more than once. 0.4% used it weekly.**

The team had shipped a technically impressive product that solved a problem nobody had, in a way nobody wanted, for users they'd never actually talked to.

This is what happens when you build without **User DNA**—the reality anchor that ensures Purpose is grounded in actual user needs, validated jobs-to-be-done, and observable behavior, not assumptions about imaginary people.

In Chapter 5, we established Purpose DNA as the "why"—the problem you exist to solve and the outcomes you pursue. But Purpose alone isn't enough. You also need to answer: **For whom? In what context? To accomplish what specific job?**

That's User DNA.

By the end of this chapter, you'll understand:
- What User DNA is and why it's the reality anchor for everything else
- How Jobs-to-be-Done (JTBD) reveals what users actually need
- How The Mom Test prevents validation theater and generates truth
- How Continuous Discovery keeps you connected to reality over time
- How to translate user research into actionable behavior archetypes
- What failure patterns emerge when User DNA is absent or fictional

Let's begin with the foundational question: Who are your users, really?

---

## What Is User DNA?

**User DNA** encodes who the product is for, the jobs they need done, and the contexts/constraints under which they operate. It replaces "imaginary users" with grounded, evidence-backed archetypes and behaviors (1).

User DNA answers five critical questions:

1. **Who are the primary and secondary users** (by behavior, not demographics)?
2. **What jobs-to-be-done (JTBD)** do they hire the product for?
3. **What triggers usage**, and what blocks adoption?
4. **What value signals** do they recognize (how do they perceive "done right")?
5. **What constraints shape their experience** (time, device, compliance, environment)?

### Why User DNA Is the Reality Anchor

Remember from Chapter 2: higher-order thinking systems operate on structured information, not gut instinct. User DNA provides that structure for understanding users.

Without User DNA:
- Teams argue from opinion: "I think users want X" vs "I think users want Y"
- Features get built based on who argues most convincingly, not what users actually need
- Validation becomes optional ("we'll test it after launch")
- The loudest stakeholder or most recent customer request drives the roadmap

With User DNA:
- Teams argue from evidence: "User research shows job X is underserved"
- Features derive from validated jobs-to-be-done
- Validation is continuous (weekly touchpoints with real users)
- Purpose DNA filters features, User DNA validates which ones actually solve user problems

This is why User DNA is the **reality anchor**: it prevents you from building products for imaginary people (2).

### The Cost of Imaginary Users

I've seen this pattern dozens of times: teams that build for "users" they've never met, in contexts they've never observed, solving problems they've never validated.

The results are predictable:

**Pattern 1: Demographic-Driven Personas**
- Team creates personas: "Sarah, 35, Marketing Manager, lives in San Francisco, likes yoga"
- Demographics tell you nothing about jobs-to-be-done or behavior
- Features get built for "Sarah" even though no one has ever met an actual Sarah
- Result: 80% of features go unused because they don't match real jobs (3)

**Pattern 2: Power User Mythology**
- Team assumes "power users" want advanced features, complexity, customization
- No data validates this assumption
- Product becomes cluttered with features 95% of users never touch
- Result: Cognitive overload for actual users, who just want core job done simply (4)

**Pattern 3: Building for Internal Stakeholders**
- Sales wants "enterprise features" to close deals
- Marketing wants "flashy demos" for campaigns
- Executives want "AI" because competitors have it
- No one asks what users are actually trying to accomplish
- Result: Feature factory building stakeholder wish lists, not user value (Chapter 3) (5)

User DNA prevents all three patterns by forcing teams to **ground every decision in observable user behavior and validated jobs**.

---

## Jobs-to-be-Done: What Users Actually Hire You For

The most powerful framework I've found for understanding users comes from Clayton Christensen's **Jobs-to-be-Done (JTBD)** theory, detailed in his book *Competing Against Luck* (6).

### The Core Insight

Christensen's principle: **"Customers don't buy products or services; they 'hire' them to do a job"** (7).

A **job** is defined as "the progress that a person is trying to make in a particular circumstance" and has **functional, social, and emotional dimensions** (8).

This is radically different from traditional feature-based thinking:

**Feature-based thinking:**
- "Our product has real-time collaboration, AI insights, and 50+ integrations"
- (Describes what the product *has*, not what job it *does*)

**Jobs-based thinking:**
- "When I'm working across time zones, I need to understand what changed while I was offline, so I can catch up quickly without reading through every message"
- (Describes progress desired, circumstance triggering need, constraints shaping solution)

Notice the difference: the first is product-centric (what we built). The second is user-centric (what progress they're trying to make).

### The McDonald's Milkshake Study: A JTBD Classic

The most famous JTBD example comes from Christensen's work with McDonald's.

**The Question**: How do we sell more milkshakes?

**Traditional approach**: Survey customers—"How can we improve our milkshakes? Thicker? More flavors? Cheaper?"

**JTBD approach**: Observe when and why customers "hire" milkshakes.

**Discovery**: 40% of milkshakes sold before 8:30am, to people buying nothing else, driving alone.

**The Job**: "Make my long, boring commute more interesting. I need something to keep one hand busy, last the whole drive, and not make a mess. I'm not even hungry yet—I just need something to do" (9).

**Implication**: The milkshake wasn't competing with other milkshakes. It was competing with bananas (too quick to eat), bagels (messy, makes fingers greasy for driving), and coffee (too hot, gone too fast).

**Solution**: Make morning milkshakes thicker (last longer), add fruit chunks (texture variety), move machine to front (faster purchase, no line). Don't compete on price or flavor—compete on "commute entertainment" job performance.

**Result**: Sales increased because the product was optimized for the actual job, not imagined preferences.

### The Four Forces of JTBD

Christensen identified **four forces** influencing whether someone "hires" your product for a job:

1. **Push of the situation**: Problems/frustrations with current solution ("My commute is boring, coffee doesn't last")
2. **Pull of the new idea**: Attraction to your product ("This milkshake will last my whole drive")
3. **Anxiety of the new**: Fear of trying something different ("What if it's too messy for driving?")
4. **Habit of the present**: Comfort with current solution ("I always just drink coffee") (10)

For someone to switch to your product:
- **Push + Pull** must outweigh **Anxiety + Habit**

This explains why technically superior products fail: they might have strong Pull but not enough Push (current solution is "good enough"), or they trigger high Anxiety ("This looks complicated"), or Habit is too strong ("I've always used X").

### Applying JTBD to Product Development

Here's how JTBD translates to product work:

**Step 1: Identify the Job** (not the feature request)
- User says: "I want a dark mode"
- JTBD question: "What job are you trying to do when you request dark mode?"
- Discovery: "When I'm working late at night, I need to reduce eye strain, so I can keep working without headaches"
- **Job**: "Reduce eye strain during extended evening work sessions"

**Step 2: Understand the Circumstance**
- When does this job arise? (Evening, after 8pm)
- What triggers it? (Lights are off, bright screen hurts eyes)
- What constraints exist? (Low ambient light, extended sessions, multiple apps open)

**Step 3: Map Competing Solutions**
- What do users currently "hire" to solve this job?
  - Reduce screen brightness (works, but reduces clarity)
  - Use f.lux/Night Shift (helps, but doesn't solve in-app brightness)
  - Stop working earlier (ideal but not realistic)
  - Wear blue-light glasses (solves some problems, creates others)

**Step 4: Evaluate Forces**
- **Push**: Current solutions partial/inadequate
- **Pull**: System-wide dark mode solves comprehensively
- **Anxiety**: Will dark mode look unprofessional? Will it break visual consistency?
- **Habit**: Users accustomed to light mode for years

**Step 5: Design Solution**
- Feature: Dark mode
- But optimized for the **job**: Reduce eye strain during evening sessions
- Design decisions informed by job:
  - Auto-switch based on time of day (removes friction)
  - High contrast maintained (solves eye strain without sacrificing clarity)
  - Preview before committing (reduces anxiety)
  - Per-app control (respects some contexts need light mode—e.g., photo editing)

Notice: the job ("reduce eye strain during evening work") led to a much richer solution than the request ("add dark mode").

### Jobs Are Multilayered: Functional, Social, Emotional

Christensen emphasizes: "A well-defined job is multilayered, requiring an engineered **set of experiences** addressing many dimensions of the job" (11).

**Example Job**: "Coordinate async work across time zones"

- **Functional dimension**: Get status updates without scheduling meetings
- **Social dimension**: Look responsive to teammates despite time zone differences
- **Emotional dimension**: Feel confident nothing critical was missed while offline

A product that only solves the functional dimension (status updates) but ignores social ("teammates think I'm unresponsive") and emotional ("anxiety about missing critical info") will fail, even if technically functional.

This is why **User DNA requires understanding all three dimensions**—not just what users need to *do*, but what they need to *feel* and how they need to be *perceived*.

---

## The Mom Test: Generating Truth, Not Validation Theater

Knowing you need to understand jobs-to-be-done is one thing. Actually getting users to tell you the truth is another.

Enter **The Mom Test** by Rob Fitzpatrick—a methodology for customer conversations that generate **truth instead of lies** (12).

### The Problem: Everyone Lies (Unintentionally)

When you ask people about your product idea, they lie. Not maliciously—they're trying to be nice, encouraging, supportive. Especially if they like you.

If you ask your mom, "Do you think this app idea is good?" she'll say "Yes, honey, it sounds wonderful!" even if it's terrible. Because she loves you.

Hence the name: **The Mom Test**—questions structured so **even your mom can't lie to you** (13).

### The Three Rules

Fitzpatrick's methodology boils down to three simple rules:

**Rule 1: Talk about their life, not your idea**
- ❌ "Would you use an app that helps you track tasks?"
- ✅ "How do you currently keep track of what you need to do?"

**Rule 2: Ask about specifics in the past, not generalizations about the future**
- ❌ "Would you pay $10/month for this?"
- ✅ "Tell me about the last time you tried to solve this problem. What did you do?"

**Rule 3: Talk less, listen more**
- ❌ Pitch your idea and ask "What do you think?"
- ✅ Ask about their experiences and shut up (14)

### Why This Works

**Rule 1** prevents validation theater. The moment you describe your idea, people start thinking, "How can I be supportive?" not "What do I actually need?"

By asking about **their life** instead, you learn about real problems, current solutions, and unmet needs—which might validate your idea, contradict it, or reveal a better opportunity.

**Rule 2** prevents hypothetical promises. "Would you pay $X?" is useless because people vastly overestimate their future behavior. What people *say* they'll do and what they *actually* do are completely different.

But "Tell me about the last time you tried to solve this" reveals **actual behavior**—what they did, what worked, what didn't, what they were willing to pay/sacrifice.

**Rule 3** prevents leading questions. If you're talking, you're not learning. The ratio should be 80% them, 20% you (mostly asking follow-up questions).

### The Mom Test in Practice

Let me show you a real conversation, before and after applying The Mom Test.

**Before (Validation Theater):**

You: "I'm building an app that helps distributed teams coordinate async work. Do you think that would be useful?"

Them: "Oh yeah, that sounds great! We struggle with coordination all the time."

You: "Would you pay $15/month per user for it?"

Them: "Probably, yeah. Sounds reasonable."

You: "Awesome! Can I add you to the beta list?"

Them: "Sure, send me the link when it's ready!"

**What you learned**: Nothing. They were polite. You have no idea if they'll actually use it or pay for it.

**After (The Mom Test):**

You: "You mentioned your team is distributed. How do you currently coordinate work across time zones?"

Them: "Uh, mostly Slack. And we have a weekly standup at 9am PST, which is rough for our London folks."

You: "Tell me about the last time coordination broke down. What happened?"

Them: "Last week, our designer started working on mockups that engineering had already decided to cut from the sprint. She spent two days on something we didn't need. Nobody told her because it happened in a Slack thread she missed."

You: "What did you try to fix that?"

Them: "We talked about maybe using Jira more, but honestly, everyone hates Jira. It's so much overhead. Some people just started recording Loom videos to explain their work, which helps, but it's not consistent."

You: "When you tried Jira, what made you stop?"

Them: "Too much process. We're a 12-person team—we don't need enterprise project management. We just need to not miss critical info when someone's working a different schedule."

**What you learned**:
- **Actual problem**: Critical info lost in async communication (validated)
- **Current solution**: Slack + weekly meeting + ad-hoc Loom videos (incomplete)
- **Push**: Designer wasted 2 days on cancelled work (strong push)
- **Anxiety**: Overhead/process (high anxiety about "enterprise tools")
- **Constraints**: Small team (12 people), need lightweight solution
- **Job-to-be-Done**: "When critical decisions happen while I'm offline, I need to be notified and brought up to speed, so I don't waste time on invalidated work"

The second conversation gives you **actionable insight**. You know what job to solve, what constraints to respect, what anxiety to avoid, and what the push/pull forces are.

### The Mom Test Guidelines (15)

Based on Fitzpatrick's work, here are practical guidelines:

**Good questions:**
- "Tell me about the last time you experienced [problem]"
- "What have you tried to solve this?"
- "What's the hardest part about [job you're exploring]?"
- "Walk me through a typical [workflow/day/session]"
- "Why did you choose [current solution]? What would make you switch?"

**Bad questions:**
- "Would you use this?" (hypothetical future)
- "How much would you pay?" (people lie)
- "What features do you want?" (users aren't product designers)
- "Do you think this is a good idea?" (politeness bias)

**Critical follow-ups:**
- "Can you tell me more about that?" (get specifics)
- "What happened next?" (understand sequence)
- "Why was that important?" (uncover emotional dimension)
- "How often does that happen?" (validate frequency)

### Academic and Industry Validation

The Mom Test isn't just indie-author wisdom—it's been validated at scale:
- **Taught at Harvard, MIT, and UCL** as core customer development methodology
- **Used as training manual at SkyScanner, Shopify**, and other high-growth companies (16)

Why? Because it solves the fundamental problem of customer conversations: they're **easy to screw up, hard to do right** (17). The Mom Test makes "hard to do right" into a simple three-rule framework.

---

## Continuous Discovery: Weekly Touchpoints with Reality

The Mom Test teaches you *how* to talk to users. But one-time user research at the beginning of a project isn't enough. You need **continuous connection to reality**.

This is where **Continuous Discovery Habits** by Teresa Torres comes in.

### What Is Continuous Discovery?

Torres defines it as: **"The process of conducting small research activities through weekly touchpoints with customers, by the team who's building the product"** (18).

Let's break that down:

**Small research activities**: Not multi-month studies. 30-60 minute interviews, usability tests, prototype validations.

**Weekly touchpoints**: Not quarterly. Not "before we build." Every single week, talk to users.

**By the team building the product**: Not outsourced to a research team. The Product Manager, Designer, and Tech Lead (the "Product Trio") conduct research themselves (19).

### Why Continuous, Not One-Time?

Traditional research pattern:
1. Spend 6 weeks doing user research upfront
2. Build for 6 months based on that research
3. Launch
4. Discover the world has changed, assumptions were wrong, or you misunderstood the job
5. Scramble to fix

Continuous Discovery pattern:
1. Talk to users weekly throughout building
2. Validate assumptions incrementally
3. Adjust course as you learn
4. Launch with high confidence
5. Continue weekly touchpoints post-launch to inform evolution

The difference: **continuous feedback loop** vs **long-delay batch feedback**.

Torres' principle: **"Outputs (features shipped) are less important than the impact you have in the lives of your customers and for your business"** (20).

Continuous Discovery ensures you're always measuring impact, not just counting outputs.

### The Product Trio

Torres recommends a **Product Trio** structure: Product Manager + Design Lead + Tech Lead working together from the beginning, making decisions collaboratively about what to build (21).

Why this structure?

- **Product Manager**: Understands business goals, user needs, strategic priorities
- **Design Lead**: Translates needs into experiences, identifies usability issues
- **Tech Lead**: Understands feasibility, technical constraints, architectural implications

When all three participate in user research:
- **Shared understanding**: No "telephone game" where research insights get distorted
- **Faster decisions**: No need to "sell" insights to stakeholders—they saw it firsthand
- **Better solutions**: Technical constraints surface early, influencing questions asked

### The Opportunity Solution Tree

Torres' practical framework for organizing continuous discovery is the **Opportunity Solution Tree** (22):

```
        Desired Outcome (North Star / OKR)
                |
        --------+--------
       |                |
   Opportunities    Opportunities
   (user needs)     (user needs)
       |                |
   Solutions        Solutions
   (features)       (features)
```

**How it works:**

1. **Start with Outcome**: What business/user outcome are you pursuing? (From Purpose DNA + OKRs)
2. **Map Opportunities**: What user needs, pain points, or jobs could drive that outcome?
3. **Generate Solutions**: For each opportunity, what features/changes could address it?
4. **Test Incrementally**: Validate opportunities (do users actually have this need?) before building solutions

**Example:**

- **Outcome**: Increase weekly active coordinated teams (WACT) by 50%
- **Opportunity 1**: "Teams don't know what changed while they were offline"
  - Solution 1a: Smart digest of updates
  - Solution 1b: Notification for critical decisions
- **Opportunity 2**: "Setting up async workflows feels like too much work"
  - Solution 2a: Pre-configured templates
  - Solution 2b: One-click workflow activation

Weekly user interviews validate:
- Is "don't know what changed" actually a blocker? (Yes? Prioritize Opportunity 1)
- Would pre-configured templates solve "too much work"? (Test prototype with 5 users)

The tree creates **traceability from outcome to solution**, ensuring every feature derives from validated opportunity.

### Teresa Torres' Impact

Torres has:
- Coached **hundreds of teams** from early-stage startups to global enterprises
- Trained **7,000+ product people** through Product Talk Academy
- Helped teams **infuse daily product decisions with customer input**, not just quarterly research (23)

Her methodology works because it makes user research **sustainable**—not a heroic effort, but a habit.

---

## Building User DNA: From Research to Archetypes

Now that you understand JTBD, The Mom Test, and Continuous Discovery, let's make this operational.

How do you translate user research into **User DNA**—the living artifact that guides product decisions?

### Step 1: Conduct JTBD Interviews (The Mom Test Style)

**Goal**: Understand jobs users are hiring products for, in their own words

**Process**:
1. Recruit 10-15 users (mix of active, churned, and prospective)
2. Use Mom Test questions focused on **past behavior**:
   - "Tell me about the last time you needed to coordinate work across time zones. What happened?"
   - "Walk me through how you currently solve [job]."
   - "What's the most frustrating part of [current solution]?"
   - "When did you last try a new tool for this? What made you stop using it?"

**Output**: Transcripts capturing:
- Jobs users are trying to get done
- Circumstances triggering those jobs
- Current solutions and their gaps
- Push/pull/anxiety/habit forces

### Step 2: Identify Patterns (Job Clustering)

**Goal**: Find recurring jobs across users

**Process**:
1. Review transcripts and extract job statements
2. Cluster similar jobs (e.g., "catch up after being offline" appears in 12/15 interviews)
3. Prioritize by frequency + intensity (how often + how painful)

**Output**: 5-7 validated jobs-to-be-done

**Example Jobs** (from async coordination research):
1. "When critical decisions happen while I'm offline, I need to be notified and brought up to speed quickly"
2. "When starting my workday, I need to understand what changed overnight without reading every message"
3. "When delegating work, I need to provide full context so teammates can act independently"
4. "When making decisions async, I need everyone's input without scheduling a meeting"
5. "When working across time zones, I need to feel responsive without being always-on"

### Step 3: Create Behavior Archetypes (Not Demographic Personas)

**Goal**: Describe users by behavior, not demographics

**Bad Persona**:
- Name: "Sarah, 35, Marketing Manager, lives in San Francisco, likes yoga"
- Problem: Demographics don't predict behavior

**Good Archetype**:
- **The Async Coordinator**: Works across 3+ time zones, manages distributed team, values documentation over meetings, frustrated by "lost context" in async communication
- **Jobs they're hiring for**: Catch up quickly, delegate with full context, make decisions without meetings
- **Value signals**: Clear notifications, searchable history, minimal cognitive load
- **Constraints**: Works 8am-5pm PST, team spans London to Sydney, high message volume

Notice: The archetype describes **behavior** (works across time zones, values documentation), **jobs** (catch up, delegate, decide), and **constraints** (specific time zones, high volume).

You can be a 22-year-old engineer or a 55-year-old executive and still be "The Async Coordinator" if you share these behavioral patterns.

**Guideline**: Create 3-5 behavior archetypes, each grounded in research

### Step 4: Map Usage Narratives (Job → Action → Outcome)

**Goal**: Describe how users accomplish jobs (current state vs desired state)

**Template**:
- **Job**: [JTBD statement]
- **Trigger**: [What prompts this need]
- **Current Approach**: [How they solve it today, 3-7 steps]
- **Pain Points**: [Where current solution fails]
- **Desired Outcome**: [What success looks like]
- **Constraints**: [Time, device, skill, compliance factors]

**Example**:

- **Job**: "When starting my workday, I need to understand what changed overnight"
- **Trigger**: Logging in after 8+ hours offline (time zone difference)
- **Current Approach**:
  1. Open Slack, scroll through channels
  2. Check email for high-priority threads
  3. Review Jira for ticket updates
  4. Ask teammates "Anything critical I missed?"
  5. Spend 20-30 minutes piecing together status
- **Pain Points**:
  - Takes 30 minutes just to "catch up" (time waste)
  - Might miss critical context buried in thread
  - Unclear what actually needs action vs just FYI
- **Desired Outcome**: Catch up in <5 minutes, confident nothing critical missed, clear actions identified
- **Constraints**: Mobile during commute (first touchpoint), limited attention span, high volume

**Guideline**: Map 5-7 usage narratives for top jobs

### Step 5: Identify Value Signals (How Users Recognize Quality)

**Goal**: Understand what users equate with "this is done right"

**Process**: During interviews, ask:
- "When you use [competitor/current solution], what makes you trust it?"
- "What would make you feel confident in a new tool?"
- "How do you know when [job] is done successfully?"

**Example Value Signals** (async coordination):
- **Speed**: Updates load in <300ms (perceived instant)
- **Reliability**: Never lose a draft, never miss a notification
- **Clarity**: Know what needs action vs what's FYI
- **Context**: Can understand decision without asking follow-ups
- **Respect**: Tool doesn't interrupt deep work for non-urgent items

**Output**: 5-10 observable signals users use to judge quality

### Step 6: Document Constraints

**Goal**: Capture environmental/situational factors shaping solutions

**Categories**:
- **Device**: Mobile vs desktop, screen size, input method
- **Time**: How much time available for task, time of day, urgency
- **Skill**: Technical proficiency, domain knowledge, training willingness
- **Compliance**: GDPR, HIPAA, SOC2, industry regulations
- **Environment**: Distractions, network quality, accessibility needs

**Example** (healthcare app):
- Device: Often mobile, sometimes gloves-on (touchscreen challenges)
- Time: 30-second windows between patients (ultra-fast interaction)
- Skill: High medical knowledge, low tech literacy
- Compliance: HIPAA-compliant, audit logging required
- Environment: Loud, bright-lit, frequent interruptions

**Output**: Constraint register per archetype

### Step 7: Create the User DNA Artifact

**Goal**: One-page living document per archetype

**Structure**:

```markdown
# Behavior Archetype: [Name]

## Who They Are (Behavioral)
- [2-3 sentences describing behavior patterns, not demographics]

## Jobs-to-be-Done (Top 3-5)
1. [Job statement with context]
2. [Job statement with context]
3. [Job statement with context]

## Value Signals (What "Quality" Means to Them)
- [Signal 1]
- [Signal 2]
- [Signal 3]

## Constraints
- Device: [typical devices/contexts]
- Time: [available time per session]
- Skill: [proficiency levels]
- Compliance: [requirements]
- Environment: [usage context]

## Usage Narrative (Primary Job)
**Trigger**: [what prompts need]
**Current Flow**: [how they solve today]
**Pain Points**: [where it fails]
**Desired Outcome**: [success state]

## Four Forces Analysis
- **Push**: [frustrations with current solution]
- **Pull**: [what would attract them to new solution]
- **Anxiety**: [fears about switching]
- **Habit**: [comfort with current approach]
```

**Guideline**: Create 3-5 User DNA artifacts (one per archetype), reviewed quarterly, updated based on continuous discovery

---

## User DNA in Action: Case Study

Let me show you User DNA transforming product development.

### Before: Demographic Personas

**Company**: "TaskFlow" (anonymized), project management SaaS, 50 employees, $12M ARR

**Personas** (created by marketing, never validated):
1. "Emma, 32, Project Manager, MBA, lives in Austin, manages 5-10 people"
2. "Carlos, 45, Engineering Lead, computer science background, San Francisco"
3. "Priya, 28, Designer, art school grad, remote worker, loves coffee shops"

**Problem**: Features were built for these personas, but no one had ever met an actual Emma, Carlos, or Priya. Demographics didn't predict behavior.

**Result**: 73% of features had <10% adoption. Churn was 42% annually.

### The Intervention: Building Real User DNA

**Process** (8 weeks):

Week 1-2: **JTBD Interviews** (Mom Test style)
- Interviewed 20 users (10 active, 5 churned, 5 prospective)
- Asked about last project coordination breakdown, current tools, pain points

Week 3-4: **Pattern Analysis**
- Identified 6 recurring jobs-to-be-done
- Found behaviors didn't correlate with demographics (age, role, location didn't predict needs)

Week 5-6: **Behavior Archetypes**
- Created 3 archetypes based on **coordination style**, not demographics:
  1. **The Delegator**: Manages distributed team, needs to provide context and track progress without micromanaging
  2. **The Executor**: Gets assigned work, needs clear expectations and autonomy to deliver
  3. **The Orchestrator**: Coordinates cross-functional initiatives, needs visibility across teams without creating overhead

Week 7-8: **Usage Narratives + Value Signals**
- Mapped how each archetype currently coordinates work
- Identified what "good coordination" looks like to each

### After: Behavior-Driven Product Development

**Changes**:

1. **Roadmap Reset**:
   - Removed 28 features built for "Emma/Carlos/Priya" that didn't map to real jobs
   - Prioritized features addressing top 3 jobs per archetype

2. **Feature Example** (The Delegator):
   - **Job**: "When delegating work, I need to provide full context so teammates can execute independently"
   - **Current pain**: Delegating via Slack or email loses context, leads to questions and delays
   - **Solution built**: "Context Cards"—rich task descriptions with linked docs, decision rationale, success criteria, embedded in task
   - **Value signals respected**: Fast to create (templates), nothing gets lost (embedded), clear expectations (success criteria explicit)

3. **Continuous Discovery**:
   - Product Trio (PM + Design + Eng Lead) interviews 3-5 users per week
   - Validates assumptions before building, not after

### Results (12 Months)

- **Feature adoption**: 73% → 58% (still work to do, but 15-point improvement)
- **Churn**: 42% → 31% (11-point drop)
- **NPS**: 28 → 44 (16-point increase)
- **Time-to-value**: 12 days → 4 days (new users hit first "job completed" faster)
- **Support tickets**: Down 35% (features aligned to jobs are more intuitive)

**Key Insight**:

The team stopped building for imaginary personas and started building for real jobs. Features went from "we think Emma would like this" to "we validated that Delegators need this to accomplish X job, and 8/10 users in testing confirmed it works."

User DNA anchored them in reality.

---

## Common User DNA Anti-Patterns

Before we close, let's address failure modes:

### Anti-Pattern 1: Personas Without Behavior

**Symptom**: Personas focused on demographics, not jobs or behavior
**Example**: "Mike, 40, VP of Sales, drives a Tesla, vacations in Cabo"
**Problem**: Demographics don't predict what jobs users hire products for
**Fix**: Behavior archetypes—describe coordination style, work patterns, job triggers, constraints

### Anti-Pattern 2: "We Don't Have Time for User Research"

**Symptom**: Team claims user research would slow them down
**Reality**: Building wrong features slows you down more
**Evidence**: 80% of features go unused (Chapter 1). That's wasted time.
**Fix**: Continuous Discovery (weekly touchpoints, 30-60 min) is faster than building wrong things

### Anti-Pattern 3: Validation Theater (Not Mom Test)

**Symptom**: Team "validates" by pitching ideas and getting polite agreement
**Example**: "Would you use this?" → "Yeah, sounds good!"
**Problem**: People lie to be polite. Hypothetical futures are unreliable.
**Fix**: The Mom Test—talk about their life, ask about past behavior, listen more than pitch

### Anti-Pattern 4: One-Time Research, Then Months of Building

**Symptom**: Research upfront, then disconnect from users during development
**Problem**: Assumptions decay, world changes, you build based on stale information
**Fix**: Continuous Discovery—weekly touchpoints throughout development, not just at beginning

### Anti-Pattern 5: Research Team Does Research, Product Team Doesn't

**Symptom**: Outsourced research creates "telephone game"
**Problem**: Insights get filtered/distorted, Product Trio doesn't develop user empathy
**Fix**: Product Trio (PM + Design + Eng) conducts research themselves

---

## Chapter Summary

**Key Points:**

1. **User DNA is the reality anchor**: It ensures Purpose is grounded in actual user needs, validated jobs-to-be-done, and observable behavior—not assumptions about imaginary people.

2. **Jobs-to-be-Done (JTBD) framework**: Customers "hire" products to make progress in particular circumstances. Jobs have functional, social, and emotional dimensions (24).

3. **Four Forces influence hiring decisions**: Push (current solution problems), Pull (new product attraction), Anxiety (fear of new), Habit (comfort with current) (25).

4. **The Mom Test generates truth**: Talk about their life (not your idea), ask about past specifics (not future hypotheticals), listen more than pitch (26).

5. **Continuous Discovery is weekly touchpoints**: Small research activities by the Product Trio (PM + Design + Tech Lead), not quarterly big studies (27).

6. **Behavior archetypes > demographic personas**: Describe users by jobs, triggers, constraints, and value signals—not age, location, or hobbies.

7. **Usage narratives map jobs to actions**: Job → Trigger → Current Approach → Pain Points → Desired Outcome → Constraints.

8. **Value signals reveal quality perception**: What users equate with "this is done right"—speed, reliability, clarity, trust indicators.

9. **User DNA is living, not static**: Updated quarterly based on continuous discovery, not set-and-forget personas.

10. **User DNA prevents feature factory syndrome**: Features derive from validated jobs, not stakeholder requests or imaginary user preferences (28).

**Practical Takeaways:**

- Conduct 10-15 JTBD interviews using The Mom Test methodology
- Identify 5-7 validated jobs-to-be-done (recurring patterns)
- Create 3-5 behavior archetypes (not demographic personas)
- Map 5-7 usage narratives (job → action → outcome)
- Document value signals (how users recognize quality)
- Establish weekly Continuous Discovery habit (Product Trio + users)
- Use Opportunity Solution Tree to map outcomes → opportunities → solutions
- Review and update User DNA quarterly based on learnings

**Next Steps:**

With Purpose DNA (Chapter 5) establishing "why we exist" and User DNA (Chapter 6) grounding us in "for whom and what jobs," we're ready for the next layer:

**Chapter 7: Experience DNA — Quality Thresholds & Flow** answers: **"What does it mean to do these jobs 'well'? What quality standards must we meet?"** Experience DNA translates Purpose and User understanding into tangible quality bars—performance thresholds, interaction patterns, accessibility standards, and the Minimum Quality Bar (MQB) that gates all releases.

**Reflection Questions:**

1. Can you articulate the top 3 jobs your users hire your product to do? (Not features, but jobs—progress they're trying to make)
2. Are your current "personas" demographic-based or behavior-based? If demographic, do they actually predict user needs?
3. When was the last time your Product Trio (PM + Design + Eng) talked to a real user? If >1 week ago, why?
4. Can you trace your current roadmap features back to validated jobs-to-be-done? Or are they based on stakeholder requests and assumptions?
5. What's preventing weekly user touchpoints? (If answer is "time," calculate time wasted building unused features.)
6. How do users currently solve the jobs your product addresses? What are they "hiring" today (including non-software solutions)?
7. What are the Four Forces for your product: Push (current solution problems), Pull (your product attraction), Anxiety (fears about switching), Habit (comfort with current)?

---

**Word Count:** ~6,100 words
**TRACE:** `SCRIPT:PART2:CH06:USER-DNA:v1.0`
**Status:** Draft Complete — Ready for Review

---

## References

1. User DNA definition adapted from Layer 1 DNA framework documentation, The Product Genome brainstorming materials.

2. Reality anchor concept synthesized from JTBD theory (Christensen) and continuous discovery practices (Torres).

3. Pendo. (2019). Feature adoption research showing 80% of features rarely/never used (referenced in Chapter 1).

4. Cognitive overload pattern observed in user research and usability testing literature (Nielsen Norman Group).

5. Perri, M. (2019). *Escaping the Build Trap*. Feature factory pattern: building stakeholder wish lists over user value.

6. Christensen, C. M., Hall, T., Dillon, K., & Duncan, D. S. (2016). *Competing Against Luck: The Story of Innovation and Customer Choice*. Harper Business.

7. THRV. (n.d.). *Clayton Christensen, Jobs-to-be-Done & Competing Against Luck, Part 1*. Retrieved from https://www.thrv.com/blog/clayton-christensen-jobs-to-be-done. Christensen quote: "Customers hire products to get a job done."

8. GoPractice. (n.d.). *Jobs to Be Done: The Theory and the Frameworks*. Retrieved from https://gopractice.io/product/jobs-to-be-done-the-theory-and-the-frameworks/. Job definition with functional, social, emotional dimensions.

9. FullStory. (n.d.). *Clayton Christensen's Jobs to Be Done Framework & Product Development*. Retrieved from https://www.fullstory.com/blog/clayton-christensen-jobs-to-be-done-framework-product-development/. McDonald's milkshake study: satiate hunger/boredom on commute.

10. CRM.org. (n.d.). *Winning the Innovation Game with Jobs-to-Be-Done Theory*. Retrieved from https://crm.org/articles/jobs-to-be-done-theory. Four Forces Framework: push, pull, anxiety, habit.

11. FullStory. (n.d.). *JTBD Framework*. Well-defined job is multilayered, requiring engineered set of experiences.

12. Fitzpatrick, R. (2013). *The Mom Test: How to Talk to Customers & Learn If Your Business Is a Good Idea When Everyone Is Lying to You*. CreateSpace Independent Publishing.

13. Looppanel. (n.d.). *The Mom Test for Better Customer Interviews*. Retrieved from https://www.looppanel.com/blog/customer-interviews. Questions even your mom can't lie about.

14. Rick Lindquist. (n.d.). *Notes and Takeaways from The Mom Test*. Retrieved from https://www.ricklindquist.com/notes/the-mom-test-by-rob-fitzpatrick. Talk about life experiences vs your idea; specifics from past vs generalizations about future.

15. Three simple rules synthesized from Fitzpatrick's *The Mom Test* methodology.

16. Nightingale Design Research. (n.d.). *Book Review: The Mom Test by Rob Fitzpatrick*. Retrieved from https://nightingaledesignresearch.com/insights/book-review-the-mom-test-by-rob-fitzpatrick/. Taught at Harvard, MIT, UCL; used at SkyScanner, Shopify.

17. Fitzpatrick, R. (2013). *The Mom Test*. Customer conversations easy to screw up, hard to do right.

18. Interaction Design Foundation. (2025). *What Is Continuous Discovery?* Retrieved from https://www.interaction-design.org/literature/topics/continuous-discovery. Torres' definition: small research activities via weekly touchpoints.

19. Mind the Product. (n.d.). *Continuous Discovery Habits*. Retrieved from https://www.mindtheproduct.com/continuous-discovery-habits/. Product Trio: PM + Design Lead + Tech Lead.

20. Mind the Product. (n.d.). *Continuous Discovery Habits*. Torres quote: "Outputs < Impact in customer lives and business."

21. Torres, T. (2021). *Continuous Discovery Habits: Discover Products That Create Customer Value and Business Value*. Product Talk Press. Product Trio structure.

22. Dovetail. (n.d.). *Continuous Discovery Habits with Teresa Torres*. Retrieved from https://dovetail.com/outlier/continuous-discovery-teresa-torres/. Opportunity Solution Tree framework.

23. Mind the Product. (n.d.). *About Teresa Torres*. Coached hundreds of teams, trained 7,000+ product people, infuse daily decisions with customer input.

24. Christensen, C. M., et al. (2016). *Competing Against Luck*. JTBD theory core principles.

25. CRM.org. (n.d.). *JTBD Theory*. Four Forces Framework.

26. Fitzpatrick, R. (2013). *The Mom Test*. Methodology summary.

27. Torres, T. (2021). *Continuous Discovery Habits*. Weekly touchpoints methodology.

28. Perri, M. (2019). *Escaping the Build Trap*. Feature factory prevention through user-centered development.

---

**END OF CHAPTER 6**

Chapter 7 explores Experience DNA—the quality thresholds, interaction patterns, and Minimum Quality Bar that ensure jobs are done *well*, not just *done*.
