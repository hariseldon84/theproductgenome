# Trace Log

**Project:** [Project Name]  
**Date Range:** [YYYY-MM-DD to YYYY-MM-DD]  
**Maintained By:** [Team/Role]

---

## Purpose

Track the provenance and lineage of AI-generated artifacts, decisions, and code throughout the product development lifecycle, enabling auditability, debugging, and learning.

---

## Trace Entry Template

**Trace ID:** [YYYY-MM-DD-NNN]  
**Timestamp:** [YYYY-MM-DD HH:MM:SS UTC]  
**AI Agent:** [Model name/version]  
**Human:** [Who interacted with AI]  
**Artifact Type:** [Code/Doc/Design/Analysis/etc.]

---

### Input (What AI Received)

**Prompt:**
```
[Full prompt provided to AI]
```

**Context Documents:**
- [Document 1 name/link]
- [Document 2 name/link]

**Previous Artifacts:**
- [Artifact 1 that this builds on]

**Constraints:**
- [Constraint 1]
- [Constraint 2]

---

### Process (How AI Worked)

**AI Model:**
- Name: [e.g., GPT-4, Claude 3, etc.]
- Version: [Model version]
- Temperature: [0.0-1.0]
- Tokens: [Input tokens / Output tokens]

**Reasoning Steps (if available):**
1. [Step 1: Understanding requirement]
2. [Step 2: Analyzing options]
3. [Step 3: Generating output]

**Source References:**
[If AI cited specific docs, code, or data, list them]

---

### Output (What AI Generated)

**Artifact Generated:**
- Type: [Code file/Document/Design/Analysis]
- Location: [File path or link]
- Size: [LOC or word count]

**Output Preview:**
```
[First 50 lines or key excerpt]
```

**Full Output Location:** [Link to file or storage]

---

### Human Review

**Reviewer:** [Name]  
**Review Date:** [YYYY-MM-DD]  
**Review Type:** Approve / Request Changes / Reject

**Review Notes:**
[What was changed, improved, or rejected]

**Changes Made:**
- [Change 1]
- [Change 2]

**Final Artifact Location:** [Updated file or document]

---

### Lineage

**Parent Artifacts (This builds on):**
- [Trace ID or artifact reference]

**Child Artifacts (This was used to create):**
- [Trace ID or artifact reference]

**Related Decisions:**
- [Decision Journal ID]

**Related Experiments:**
- [Experiment Pack ID]

---

### Metadata

**Tags:** [AI-generated, reviewed, production, deprecated, etc.]  
**Quality Score:** [1-10 from human review]  
**Iteration Count:** [How many revisions]  
**Time to Approval:** [Time from generation to approval]

---

## Trace Log (Index)

| Trace ID | Date | Artifact Type | AI Agent | Human | Status | Quality |
|----------|------|--------------|---------|-------|--------|---------|
| 2025-01-15-001 | 2025-01-15 | PRD | GPT-4 | Alice | Approved | 8/10 |
| 2025-01-15-002 | 2025-01-15 | User Story | GPT-4 | Bob | In Review | TBD |
| 2025-01-14-003 | 2025-01-14 | Code (API endpoint) | Claude | Charlie | Approved | 9/10 |
| [ID] | [Date] | [Type] | [AI] | [Human] | [Status] | [Score] |

---

## Artifact Lineage Map

**Visual representation of how artifacts relate:**

```
PRD (2025-01-10-001)
  └── Architecture Doc (2025-01-11-002)
       └── User Story 1.1 (2025-01-12-003)
            ├── Code: API endpoint (2025-01-14-004)
            │    └── Unit Tests (2025-01-15-005)
            └── Code: UI Component (2025-01-14-006)
                 └── Integration Test (2025-01-15-007)
```

**Purpose:** Understand dependencies, trace issues back to source, assess impact of changes.

---

## AI Model Performance Tracking

**By Model:**
| Model | Artifacts Generated | Avg Quality Score | Approval Rate | Avg Iterations | Avg Time to Approval |
|-------|-------------------|------------------|---------------|---------------|---------------------|
| GPT-4 | [N] | [X/10] | [Y%] | [Z] | [W hours] |
| Claude | [N] | [X/10] | [Y%] | [Z] | [W hours] |

**By Artifact Type:**
| Artifact Type | Artifacts Generated | Avg Quality Score | Approval Rate |
|--------------|-------------------|------------------|---------------|
| PRD | [N] | [X/10] | [Y%] |
| User Story | [N] | [X/10] | [Y%] |
| Code | [N] | [X/10] | [Y%] |
| Test | [N] | [X/10] | [Y%] |
| Architecture | [N] | [X/10] | [Y%] |

---

## Quality Trend Analysis

**Quality Score Over Time:**
| Month | Avg Quality | Artifacts Generated | Approval Rate |
|-------|------------|-------------------|---------------|
| 2025-01 | [X/10] | [N] | [Y%] |
| 2024-12 | [X/10] | [N] | [Y%] |

**Trend:** ⬆️ Improving / ➡️ Stable / ⬇️ Declining

**Why?**
[Analysis of what's driving quality changes: better prompts, model improvements, human review rigor, etc.]

---

## AI Contribution by Category

| Category | AI-Generated | Human-Generated | Hybrid | % AI Contribution |
|----------|-------------|-----------------|--------|-------------------|
| Requirements | [N] | [N] | [N] | [X%] |
| Architecture | [N] | [N] | [N] | [X%] |
| Design | [N] | [N] | [N] | [X%] |
| Code | [N] | [N] | [N] | [X%] |
| Tests | [N] | [N] | [N] | [X%] |
| Documentation | [N] | [N] | [N] | [X%] |

**Overall AI Contribution:** [X]% of artifacts have AI involvement

**Hybrid Definition:** AI generated draft, human significantly revised

---

## Failure Mode Analysis

**AI-Generated Artifacts That Failed Review:**
| Trace ID | Artifact Type | Failure Reason | Root Cause | Improvement |
|----------|--------------|---------------|-----------|------------|
| [ID] | [Type] | [Why rejected] | [What went wrong] | [How to prevent] |

**Common Failure Modes:**
1. [Failure mode 1] — Frequency: [N times] — Fix: [Solution]
2. [Failure mode 2] — Frequency: [N times] — Fix: [Solution]

**Example:**
- **Failure Mode:** AI-generated code missing error handling
- **Frequency:** 10 times
- **Root Cause:** Prompts didn't explicitly request error handling
- **Fix:** Update prompt templates to include "ensure comprehensive error handling for all edge cases"

---

## Prompt Effectiveness Tracking

**Prompt-to-Quality Correlation:**
| Prompt Type | Avg Quality Score | Approval Rate | Iterations |
|------------|------------------|---------------|-----------|
| [Prompt pattern from Prompting Playbook] | [X/10] | [Y%] | [Z] |

**Most Effective Prompts:**
1. [Prompt type] — Quality: [X/10] — Approval: [Y%]
2. [Prompt type] — Quality: [X/10] — Approval: [Y%]

**Least Effective Prompts:**
1. [Prompt type] — Quality: [X/10] — Approval: [Y%]
2. [Prompt type] — Quality: [X/10] — Approval: [Y%]

**Action:** Update Prompting Playbook based on these findings.

---

## Audit Queries

**Common Audit Questions:**

**Q1: Show all artifacts related to [Feature X]**
```sql
SELECT * FROM trace_log WHERE tags LIKE '%feature-x%';
```

**Q2: Which AI-generated code is in production?**
```sql
SELECT * FROM trace_log 
WHERE artifact_type = 'Code' 
  AND tags LIKE '%production%';
```

**Q3: What artifacts did [Human Y] review?**
```sql
SELECT * FROM trace_log WHERE human = 'Human Y';
```

**Q4: Show lineage of [Artifact Z]**
```sql
-- Recursive query to show parent and child artifacts
```

---

## Compliance & Governance

**AI Artifact Audit Trail:**
- All AI-generated artifacts logged with trace ID
- All prompts and outputs stored
- All human reviews documented
- All changes tracked

**Retention Policy:**
- Trace logs retained for [X years]
- Full artifacts retained for [Y years]
- Compressed archives after [Z years]

**Access Control:**
- Who can view trace logs: [Roles]
- Who can modify trace logs: [Roles]
- Who can delete trace logs: [Roles]

**Regulatory Compliance:**
[If applicable, note any compliance requirements: GDPR, SOC 2, ISO, etc.]

---

## AI Contribution Attribution

**For reporting AI productivity gains:**

| Developer | Artifacts Created | % AI-Assisted | Time Saved (est.) | Quality Impact |
|-----------|------------------|--------------|-------------------|----------------|
| Alice | [N] | [X%] | [Y hours] | [+/-Z%] |
| Bob | [N] | [X%] | [Y hours] | [+/-Z%] |

**Team-Level Metrics:**
- Total artifacts created: [N]
- % AI-assisted: [X%]
- Est. time saved: [Y hours]
- Quality impact: [+/-Z% defect rate change]

---

## Trace Examples

### Example 1: AI-Generated PRD

**Trace ID:** 2025-01-10-001  
**Timestamp:** 2025-01-10 14:30:00 UTC  
**AI Agent:** GPT-4  
**Human:** Alice (PM)  
**Artifact Type:** PRD

**Input Prompt:**
```
[CONTEXT]
We are building a task management SaaS for small teams. Users need to see which tasks depend on others to understand what's blocking progress.

[ROLE]
Act as a Product Manager with expertise in productivity tools.

[ACTION]
Create a PRD for "Task Dependencies" feature. Include user stories, acceptance criteria, success metrics.

[FORMAT]
Use markdown with H2 sections, tables for ACs.

[TONE]
Clear, actionable for engineering team.
```

**AI Output:** [Link to generated PRD]

**Human Review:**
- Reviewer: Alice
- Changes: Added edge case for circular dependencies, refined success metrics
- Quality Score: 8/10
- Status: Approved

**Lineage:**
- Child: Architecture Doc (2025-01-11-002)
- Child: User Story 1.1 (2025-01-12-003)

---

### Example 2: AI-Generated Code

**Trace ID:** 2025-01-14-004  
**Timestamp:** 2025-01-14 10:15:00 UTC  
**AI Agent:** Claude 3  
**Human:** Charlie (Dev)  
**Artifact Type:** Code (API endpoint)

**Input Prompt:**
```
[CONTEXT]
User story 1.1: Users can link tasks with dependencies. API needs to accept task ID and list of dependency task IDs, validate no cycles, update DB.

[ACTION]
Generate Node.js Express API endpoint: POST /api/tasks/:id/dependencies

[CONSTRAINTS]
- Use existing Task model (sequelize)
- Detect cycles with DFS algorithm
- Return 400 if cycle detected
- Include comprehensive error handling
- Follow our REST conventions

[FORMAT]
Show code with inline comments, plus separate unit test file.
```

**AI Output:** [Link to generated code]

**Human Review:**
- Reviewer: Charlie
- Changes: Optimized cycle detection, added transaction wrapper
- Quality Score: 9/10
- Status: Approved, merged to main

**Lineage:**
- Parent: User Story 1.1 (2025-01-12-003)
- Child: Unit Tests (2025-01-15-005)

---

## Review Cadence

- **Daily:** Add new trace entries as AI artifacts are generated
- **Weekly:** Review AI performance metrics, identify failure modes
- **Monthly:** Analyze trends, update prompting strategies, report AI contribution
- **Quarterly:** Full audit, compliance check, retention policy review

---

**TRACE:** L4:NCO:TraceLog  
**Cross-ref:** Collaboration Charter, Decision Journal, Prompting Playbook, Data DNA (L1)
