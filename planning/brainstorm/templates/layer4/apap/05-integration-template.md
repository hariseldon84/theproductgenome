# APAP Template: Integration Template

Purpose: Define external/internal integration points with stability and safety.

## Integration Point
- Name:
- Type: REST | GraphQL | Webhook | SDK | Queue
- Direction: inbound/outbound

## Contracts
- Endpoint/Topic:
- Auth:
- Payloads:
- Error handling:

## Compatibility
- Versioning strategy
- Rate limits
- Retries + backoff

## Observability
- Health checks
- Dead letter queues
- Alerting

## Risks
- Breaking changes
- SLA breaches

## Ready-to-Generate Prompt
```
Goal: Integrate with <service>
Define: endpoints, auth, payloads, retries
Constraints: respect rate limits, versioning
Validation: contract tests + integration tests
```