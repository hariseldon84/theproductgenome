# APAP Template: Schema Sheet

Purpose: Define data contracts with validation, evolution notes, and lineage.

## Entities
- Entity: `Name`
  - Fields: name:type:constraints
  - Indexes:
  - Relations:

## Validation Rules
- Field-level: regex/range/enums
- Cross-entity constraints

## API Contracts
- POST /entity: request/response
- GET /entity/:id
- Error codes

## Migration Plan
- Version: v1 → v1.1
- Additive changes only (prefer)
- Backward compatibility notes

## Observability
- Events emitted
- Metrics
- Audit fields

## Risks & Mitigations
- Data loss → backups
- Hot path queries → indexes

## Ready-to-Generate Prompt
```
Goal: Create schemas + API contracts
Entities: <list>
Rules: <validation>
Migrations: <plan>
Observability: <events/metrics>
Constraints: additive, backwards-compatible
```