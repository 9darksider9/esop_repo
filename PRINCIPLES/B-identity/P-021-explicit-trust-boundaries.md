# P-021 Explicit Trust Boundaries

## Statement

Trust boundaries must be explicit and documented.

## Reasoning

Implicit trust relationships create unexamined attack paths. When trust
boundaries are undocumented, security teams cannot identify lateral
movement risks, architects cannot evaluate boundary violations, and
operators cannot enforce boundary controls.

Explicit documentation forces deliberate trust decisions and enables
systematic boundary enforcement.

## Justification

Major breaches consistently exploit trust relationships that were
assumed but never examined. Flat networks, inherited permissions, and
undocumented integrations all represent implicit trust that attackers
exploit. You cannot defend boundaries you have not identified.

## Operational Uses

- Trust boundary documentation in architecture artifacts.
- Boundary enforcement through segmentation controls.
- Regular review of documented boundaries versus actual state.
- Cross-boundary access requires explicit approval.
- Boundary changes subject to security review.

## Misuse / Abuse Risks

- Documentation becoming stale as systems evolve.
- Excessive boundary creation adding operational friction.
- Boundaries on paper not enforced technically.
- Boundary complexity obscuring actual trust relationships.

## Related Principles

- P-022 Cross-Boundary Telemetry
- P-036 Blast Radius Measurable
- P-037 Lateral Movement Visible

## Compliance Touchpoints

Placeholder
