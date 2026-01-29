# P-038 Shared Fate Justification

## Statement

Shared fate systems require explicit justification.

## Reasoning

Systems that share failure modes—shared credentials, shared
infrastructure, shared dependencies—multiply blast radius. When one
fails or is compromised, all fail. Shared fate must be a deliberate
choice with documented justification, not an accident of convenience.

Convenience is not justification for shared fate.

## Justification

Organizations often discover shared fate during incidents when a single
compromise cascades across many systems. Shared fate created for
operational convenience creates systemic vulnerability. Explicit
justification forces evaluation of whether shared fate is worth its
risk.

## Operational Uses

- Shared fate analysis in architecture reviews.
- Credential scope limiting shared fate exposure.
- Dependency management to limit shared infrastructure.
- Risk acceptance documentation for shared fate decisions.
- Shared fate reduction as an architectural goal.

## Misuse / Abuse Risks

- Excessive isolation increasing operational complexity.
- Justification becoming pro-forma approval.
- Cost of eliminating shared fate exceeding risk benefit.
- Ignoring efficiency benefits of appropriate sharing.

## Related Principles

- P-036 Blast Radius Measurable
- P-021 Explicit Trust Boundaries
- P-035 Assume Compromise

## Compliance Touchpoints

Placeholder
