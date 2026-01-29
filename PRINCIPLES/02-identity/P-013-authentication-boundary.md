# P-013 Authentication Boundary

## Statement

Trust boundaries require re-authentication; implicit trust does not
cross zones.

## Reasoning

Network position, prior authentication, or session state in one zone
does not establish identity in another. Each trust boundary represents
a potential compromise point where an attacker may have gained access.
Re-authentication ensures that the entity crossing the boundary is still
the authorized actor.

Implicit trust propagation allows attackers to pivot from low-value
footholds to high-value targets without additional friction.

## Justification

Lateral movement attacks depend on trust relationships that allow
authenticated sessions to access resources across boundaries without
re-verification. Compromised workstations access servers. Compromised
applications access databases. Each hop inherits trust from the previous
authentication without validating current legitimacy.

Zero-trust architectures eliminate implicit trust to contain breaches.

## Operational Uses

- Segmentation with authentication at zone boundaries.
- Step-up authentication for sensitive operations.
- Session validation on cross-boundary requests.
- Mutual authentication between services.
- Token scope limiting to specific trust zones.

## Misuse / Abuse Risks

- User friction from excessive re-authentication prompts.
- Performance overhead from repeated authentication.
- Complexity in distributed systems with many boundaries.
- Inconsistent enforcement creating false confidence.

## Related Principles

- P-010 Attributable Identity
- P-012 Least Privilege
- P-032 Blast Radius Containment

## Compliance Touchpoints

Placeholder
