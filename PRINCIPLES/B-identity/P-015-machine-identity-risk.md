# P-015 Machine Identity Risk

## Statement

Machine identities are more dangerous than human identities.

## Reasoning

Machine identities operate at scale, around the clock, without fatigue
or oversight. A compromised machine identity can perform thousands of
actions before detection. Machine credentials often have broader
access than human credentials and are frequently overlooked in access
reviews.

Machine identity management requires the same rigor as human identity
management—or more.

## Justification

Service accounts, API keys, and automation credentials are primary
targets for attackers because they provide persistent, automated access.
Machine identities often lack MFA, have weak rotation, and are shared
across systems. Breaches increasingly pivot through machine credentials
rather than human credentials.

## Operational Uses

- Machine identity inventory and ownership assignment.
- Rotation requirements for all machine credentials.
- Scope limitation for machine identity permissions.
- Anomaly detection for machine identity usage patterns.
- Lifecycle management for deprovisioning unused machine identities.

## Misuse / Abuse Risks

- Rotation frequency breaking dependent automation.
- Scope restrictions preventing legitimate automation.
- Inventory overhead for dynamic environments.
- Over-monitoring creating alert fatigue.

## Related Principles

- P-016 Credential Hygiene
- P-017 Standing Privilege Debt
- P-018 Privilege Decay

## Compliance Touchpoints

Placeholder
