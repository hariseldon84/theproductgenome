# APAP Template: Frontend Golden Path Spec

Purpose: Define a crisp, mobile-first spec AI can implement safely.

## Context
- Tech stack: (e.g., Next.js + TypeScript + Tailwind)
- Design system: (tokens, components)
- Accessibility targets: WCAG 2.1 AA

## Page/Flow
- Title:
- User goal:
- Primary actions:

## Structure
- Route: `/...`
- Components:
  - `ComponentName`: props, state, events
- Data sources:
  - API: method, path, payload, response

## Mobile → Desktop
- Mobile layout:
- Tablet adjustments:
- Desktop adjustments:

## States
- Loading:
- Empty:
- Error:
- Success:

## Constraints
- Do NOT modify: `Navbar`, `AuthContext`, global styles
- Only create/edit: `pages/...`, `components/...`

## Validation
- Unit: component renders, event handlers
- Integration: API call success/error
- E2E: user completes flow

## Ready-to-Generate Prompt
```
Goal: Build <page/flow>
Steps:
1) Create files: ...
2) Implement components with props: ...
3) Wire API: ...
4) Add states: loading/empty/error/success
5) Write tests: unit/integration/e2e
Constraints: Only change listed files
```