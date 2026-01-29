# P-021 Idempotent Operations

## Statement

Automated operations must be safely repeatable without unintended side
effects.

## Reasoning

Automation fails. Networks partition. Systems crash mid-operation.
Operators retry. If operations are not idempotent, retries cause
corruption, duplication, or cascading failures.

Security automation must be designed so that repeated execution produces
the same end state as single execution. This enables safe retries,
self-healing, and convergent configuration.

## Justification

Non-idempotent operations create fragile systems where failure recovery
requires manual intervention and state forensics. Security remediation
that cannot be safely retried slows incident response. Configuration
management that diverges on retry creates inconsistent security posture.

Idempotency is a prerequisite for reliable automation at scale.

## Operational Uses

- Configuration management that converges to desired state.
- Remediation scripts that check state before acting.
- Provisioning pipelines that handle partial completion.
- Cleanup operations that tolerate missing resources.
- Event processors that deduplicate on replay.

## Misuse / Abuse Risks

- Assuming idempotency without testing edge cases.
- Hidden state dependencies that break idempotency guarantees.
- Performance overhead from state verification.
- Complexity in systems with external side effects.

## Related Principles

- P-020 Automation Default
- P-022 Audit Trail Mandatory
- P-071 Rollback Capability

## Compliance Touchpoints

Placeholder
