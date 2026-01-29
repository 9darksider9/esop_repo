# IDN-02.14 — Boundary Enforcement

## Statement

Third-party access must be segmented, scoped, and monitored; implicit
trust across boundaries is prohibited.

## Reasoning

Third parties require access to provide value, but that access creates
risk. Boundary enforcement limits third-party access to minimum required
scope, segments it from internal resources, and monitors it for anomalies.
Implicit trust allows third-party compromises to become organizational
compromises.

Third-party boundaries must be as rigorous as external boundaries.

## Justification

Breaches frequently propagate through third-party connections that were
granted broad access for operational convenience. Compromised vendors
access internal systems through trusted connections. Attackers target
third parties specifically to pivot into their customers.

Least-privilege and segmentation principles apply to third parties as
they do to internal users.

## Operational Uses

- Dedicated network segments for third-party access.
- Scoped credentials with minimum necessary permissions.
- Enhanced monitoring of third-party sessions.
- Time-bounded access for specific engagements.
- Separate authentication for third-party integrations.

## Misuse / Abuse Risks

- Operational friction from excessive access restrictions.
- Segmentation gaps from legacy or emergency integrations.
- Monitoring blind spots in encrypted third-party channels.
- Workarounds that bypass intended boundaries.

## Related Principles

- IDN-02.01 Authentication Boundary
- RES-04.02 Blast Radius Containment
- ETH-06.08 Vendor Assessment

## Compliance Touchpoints

Placeholder
