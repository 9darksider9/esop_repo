# P-018 Privilege Decay

## Statement

Privilege accumulation without decay is a defect.

## Reasoning

Access naturally expands as systems evolve and people change roles.
Without enforced decay, permissions accumulate indefinitely, creating
latent privilege exposure and unintended access paths.

Security requires continuous contraction of privilege, not periodic
cleanup.

## Justification

Most lateral movement exploits stale access: forgotten admin roles,
orphaned service accounts, unused API tokens, inherited permissions,
and abandoned group memberships. Manual access reviews rarely remove
enough access to counter natural growth.

## Operational Uses

- Automatic entitlement expiration.
- Drift detection pipelines.
- Privilege age scoring.
- Just-in-time elevation workflows.
- Access recertification with removal defaults.

## Misuse / Abuse Risks

- Over-aggressive expiration disrupting operations.
- Excessive approval friction if automation is weak.
- Shadow access creation to bypass controls.
- Decay policies that don't match operational rhythms.

## Related Principles

- P-013 Attributable Identity
- P-017 Standing Privilege Debt
- P-024 Workload-Based Privilege

## Compliance Touchpoints

Placeholder
