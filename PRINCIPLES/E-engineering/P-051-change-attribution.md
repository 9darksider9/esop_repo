# P-051 Change Attribution

## Statement

Change must be attributable.

## Reasoning

Every change to a system must be traceable to who made it, when, and
under what authority. Unattributed changes cannot be distinguished
from attacker modifications, cannot be investigated during incidents,
and cannot be held accountable for their consequences.

Unattributed change is unauthorized change.

## Justification

Attackers seek to make changes that cannot be traced back to them.
Legitimate changes that lack attribution create cover for malicious
changes. Incident responders who cannot attribute changes cannot scope
compromises. Attribution is the foundation of change accountability.

## Operational Uses

- Audit logging for all configuration and code changes.
- Identity binding for change automation.
- Change approval records linked to changes.
- Version control attribution for all repositories.
- Privileged action attribution requirements.

## Misuse / Abuse Risks

- Attribution overhead for high-frequency changes.
- Shared automation credentials obscuring true attribution.
- Attribution used for blame rather than learning.
- Privacy concerns from detailed change tracking.

## Related Principles

- P-013 Attributable Identity
- P-050 Configuration Is Code
- P-049 Drift Detection

## Compliance Touchpoints

Placeholder
