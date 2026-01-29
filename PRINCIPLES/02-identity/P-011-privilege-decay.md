# P-011 Privilege Decay

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
orphaned service accounts, unused API tokens, inherited permissions, and
abandoned group memberships. Manual access reviews rarely remove enough
access to counter natural growth.

## Operational Uses

- Automatic entitlement expiration.
- Drift detection pipelines.
- Privilege age scoring.
- Just-in-time elevation workflows.

## Misuse / Abuse Risks

- Over-aggressive expiration disrupting operations.
- Excessive approval friction if automation is weak.
- Shadow access creation to bypass controls.

## Related Principles

- P-010 Attributable Identity
- P-012 Least Privilege

## Compliance Touchpoints

Placeholder
