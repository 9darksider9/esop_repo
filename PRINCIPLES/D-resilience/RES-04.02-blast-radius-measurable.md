# RES-04.02 — Blast Radius Measurable

## Statement

Blast radius must be measurable.

## Reasoning

If you cannot measure the potential impact of a compromise, you cannot
design effective containment. Blast radius—the scope of damage from a
single point of failure or compromise—must be quantifiable for each
system, credential, and trust relationship.

Unmeasurable blast radius is unbounded blast radius.

## Justification

Organizations consistently underestimate blast radius until a real
incident reveals the true scope. Shared credentials, implicit trust,
and undocumented dependencies all extend blast radius beyond obvious
boundaries. Measurement forces explicit accounting of these
relationships.

## Operational Uses

- Blast radius analysis in architecture reviews.
- Credential scope mapping and limitation.
- Dependency graphs showing failure propagation paths.
- Impact assessment for critical systems.
- Blast radius reduction as a security objective.

## Misuse / Abuse Risks

- Measurement complexity creating analysis paralysis.
- False precision in inherently uncertain estimates.
- Measurement overhead delaying security improvements.
- Ignoring unmeasurable but real blast radius.

## Related Principles

- RES-04.01 Assume Compromise
- RES-04.03 Lateral Movement Visible
- RES-04.04 Shared Fate Justification

## Compliance Touchpoints

Placeholder
