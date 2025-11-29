# Naming Consistency Registry

**Project:** [Project Name]  
**Version:** [X.Y]  
**Last Updated:** [YYYY-MM-DD]  
**Maintained By:** [Team/Role]

---

## Purpose

Establish and enforce consistent naming conventions across all layers of the product to reduce cognitive load and improve code/UI clarity.

---

## Naming Principles

1. **Clarity over Brevity** — Prefer descriptive names even if longer
2. **Consistency over Convention** — Once a pattern is chosen, use it everywhere
3. **Semantic Alignment** — Names should reflect mental models from Semantic Layer Map
4. **Context Appropriateness** — Adjust verbosity based on scope
5. **Avoid Jargon** — Unless domain-specific and universally understood

---

## UI Naming Conventions

### Buttons & Actions

| Pattern | Example | Use When |
|---------|---------|----------|
| Verb + Noun | "Create Project" | Primary actions |
| Noun (implied action) | "Settings" | Navigation |
| Verb | "Save" / "Cancel" | Form actions |
| Icon + Verb | "🗑️ Delete" | Destructive actions (icon adds clarity) |

**Approved Verbs:**
- Create, Add, New (for creation)
- Edit, Update, Modify (for changes)
- Delete, Remove (for deletion)
- Save, Submit (for persistence)
- Cancel, Close (for dismissal)

**Forbidden:**
- ❌ "OK" / "Yes" (too vague)
- ❌ "Do it" / "Go" (unclear action)
- ❌ "Submit" for destructive actions

---

### Form Fields

| Pattern | Example | Use When |
|---------|---------|----------|
| Noun or Noun Phrase | "Email Address" | Simple fields |
| Question Format | "What's your email?" | Conversational UI |
| Instructional | "Enter your password" | When guidance needed |

**Rules:**
- Labels should end without punctuation unless a question
- Required fields: Use asterisk (*) or "(required)" suffix
- Optional fields: Use "(optional)" suffix or assume all required unless stated

---

### Status & State Labels

| State Type | Pattern | Examples |
|------------|---------|----------|
| Boolean States | Active/Inactive, Enabled/Disabled | "Active", "Disabled" |
| Progress States | Gerund (-ing form) | "Processing", "Loading" |
| Completion States | Past tense | "Completed", "Failed" |
| Pending States | "Pending [action]" | "Pending Approval" |

---

### Navigation & Sections

| Pattern | Example | Use When |
|---------|---------|----------|
| Plural Nouns | "Projects", "Settings" | Collections |
| Singular Nouns | "Profile", "Dashboard" | Single entities |
| Activity Nouns | "Activity", "History" | Event logs |

---

## API Naming Conventions

### Endpoints

**Pattern:** `/api/v{version}/{resource-plural}/{id?}/{action?}`

| Example | Purpose |
|---------|---------|
| `/api/v1/projects` | List all projects (GET) / Create project (POST) |
| `/api/v1/projects/123` | Get/Update/Delete specific project |
| `/api/v1/projects/123/archive` | Custom action on resource |

**Rules:**
- Use plural nouns for resources
- Use kebab-case for multi-word resources: `/project-templates`
- Avoid verbs in endpoint paths (use HTTP methods)
- Actions use verb form: `/activate`, `/archive`

---

### JSON Property Names

**Pattern:** `camelCase` for all properties

| Category | Pattern | Examples |
|----------|---------|----------|
| Simple Properties | camelCase noun | `firstName`, `emailAddress` |
| Boolean Properties | `is` + Adjective or `has` + Noun | `isActive`, `hasPermission` |
| Timestamps | `[event]At` | `createdAt`, `updatedAt`, `deletedAt` |
| Collections | Plural noun | `projects`, `users` |
| IDs | `id` or `[resource]Id` | `id`, `userId`, `projectId` |

**Examples:**
```json
{
  "id": "uuid",
  "firstName": "string",
  "isActive": true,
  "createdAt": "2025-11-29T10:00:00Z",
  "projects": [
    {
      "id": "uuid",
      "projectName": "string"
    }
  ]
}
```

---

## Code Naming Conventions

### Variables

**Pattern:** Based on language conventions

**JavaScript/TypeScript:**
```javascript
// camelCase for variables and functions
const userEmail = "user@example.com";
let isProcessing = false;

// PascalCase for classes and types
class ProjectManager {}
type UserProfile = {};

// UPPER_SNAKE_CASE for constants
const MAX_RETRY_ATTEMPTS = 3;
const API_BASE_URL = "https://api.example.com";
```

**Python:**
```python
# snake_case for variables and functions
user_email = "user@example.com"
is_processing = False

# PascalCase for classes
class ProjectManager:
    pass

# UPPER_SNAKE_CASE for constants
MAX_RETRY_ATTEMPTS = 3
```

---

### Functions/Methods

| Pattern | Example | Use When |
|---------|---------|----------|
| Verb + Noun | `getUser()`, `createProject()` | Actions |
| Verb + Adjective | `isValid()`, `hasPermission()` | Boolean return |
| Noun (getter convention) | `user()`, `email()` (in languages with property-like methods) | Accessors |

**Approved Verbs:**
- **CRUD:** `create`, `get`/`fetch`, `update`, `delete`/`remove`
- **Queries:** `find`, `list`, `search`, `filter`
- **Validation:** `validate`, `check`, `verify`
- **Conversion:** `to[Type]`, `from[Type]`, `parse`, `format`
- **Computation:** `calculate`, `compute`, `generate`

---

### Classes/Types

| Pattern | Example | Use When |
|---------|---------|----------|
| Noun (Singular) | `User`, `Project`, `EmailService` | Entities |
| Adjective + Noun | `ActiveUser`, `PendingProject` | Specific states |
| Noun + Noun | `ProjectManager`, `EmailValidator` | Functional units |
| `I` + Noun (Interface) | `IUserRepository`, `IEmailService` | Interfaces (some languages) |

---

### Files/Modules

| Pattern | Example | Use When |
|---------|---------|----------|
| kebab-case | `user-service.ts`, `email-validator.ts` | File names |
| PascalCase | `UserService.ts`, `EmailValidator.ts` | Class-based modules (if convention) |
| index | `index.ts`, `__init__.py` | Module entry points |

---

## Database Naming Conventions

### Tables

**Pattern:** `snake_case`, plural nouns

| Example | Purpose |
|---------|---------|
| `users` | User records |
| `project_members` | Join table |
| `email_templates` | Template records |

---

### Columns

**Pattern:** `snake_case`

| Category | Pattern | Examples |
|----------|---------|----------|
| Primary Key | `id` | `id` |
| Foreign Key | `[table_singular]_id` | `user_id`, `project_id` |
| Boolean | `is_[adjective]` or `has_[noun]` | `is_active`, `has_permission` |
| Timestamps | `[event]_at` | `created_at`, `updated_at` |

---

## Test Naming Conventions

### Test Files

**Pattern:** `[module-name].test.ts` or `test_[module_name].py`

---

### Test Functions/Methods

**Pattern:** `test_[should]_[expected_behavior]_[when_condition]`

**Examples:**
```javascript
// JavaScript/TypeScript
describe('UserService', () => {
  it('should create user when valid data provided', () => {});
  it('should throw error when email is invalid', () => {});
});
```

```python
# Python
def test_should_create_user_when_valid_data_provided():
    pass

def test_should_throw_error_when_email_is_invalid():
    pass
```

---

## Consistency Audit

### Cross-Layer Terminology Check

| Concept | UI Label | API Property | Code Variable | Database Column | Status |
|---------|----------|--------------|---------------|-----------------|--------|
| User's email | "Email Address" | `emailAddress` | `emailAddress` | `email_address` | ✅ |
| Project status | "Status" | `status` | `status` | `status` | ✅ |
| [Concept] | [Term] | [Term] | [Term] | [Term] | ✅/❌ |

---

### Naming Violations Log

| Location | Current Name | Issue | Correct Name | Priority | Owner | Status |
|----------|--------------|-------|--------------|----------|-------|--------|
| [File:Line] | [Name] | [Why wrong] | [Correct name] | 🔴/🟡/🟢 | [Name] | Open/Fixed |

---

## Naming Decision Log

When naming decisions are contested or ambiguous, document the decision here:

### Decision: [Topic - e.g., "User vs Account"]

**Date:** [YYYY-MM-DD]  
**Decision:** Use "[chosen term]"  
**Rationale:** [Why this choice]  
**Alternatives Considered:** [Other options]  
**Scope:** [Where this applies]  
**Approved By:** [Name/Role]

---

## Linting & Enforcement

### Automated Checks

**ESLint/TSLint (JavaScript/TypeScript):**
```json
{
  "rules": {
    "camelcase": ["error", { "properties": "always" }],
    "naming-convention": [
      "error",
      {
        "selector": "variable",
        "format": ["camelCase", "UPPER_CASE"]
      },
      {
        "selector": "function",
        "format": ["camelCase"]
      },
      {
        "selector": "class",
        "format": ["PascalCase"]
      }
    ]
  }
}
```

**pylint (Python):**
```ini
[BASIC]
variable-naming-style=snake_case
function-naming-style=snake_case
class-naming-style=PascalCase
const-naming-style=UPPER_CASE
```

---

### Code Review Checklist

- [ ] Variable names are descriptive and follow conventions
- [ ] Function names use approved verbs
- [ ] Boolean variables use `is`/`has` prefix
- [ ] Class names are nouns in PascalCase
- [ ] No abbreviations unless approved
- [ ] Consistent terminology with Semantic Layer Map
- [ ] Test names describe behavior clearly

---

## Reference Quick Links

- Semantic Layer Map: [Link]
- API Standards: [Link]
- Code Style Guide: [Link]
- UI Copy Guidelines: [Link]

---

**TRACE:** L4:CognitiveLoad:Naming  
**Cross-ref:** Semantic Layer Map, Cognitive Load Audit, Experience DNA (L1), Architecture DNA (L1)
