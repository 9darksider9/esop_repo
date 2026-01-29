# IDN-02.13 — Least Privilege

## Statement

Access defaults to denied; grants must be explicit, scoped, and
justified.

## Reasoning

Excessive privilege creates unnecessary attack surface. Every permission
beyond minimum required represents potential for misuse, lateral
movement, or accidental damage. Default-deny forces explicit decisions
about what access is necessary.

Scoped grants limit blast radius. Justified grants create accountability
and enable review. Implicit or inherited access bypasses these controls.

## Justification

Most privilege escalation attacks exploit overly permissive defaults,
inherited roles, or convenience-driven broad grants. Attackers seek
accounts with more access than their function requires because excess
privilege enables lateral movement without additional exploitation.

Access accumulation over time compounds the problem. Without
least-privilege enforcement, organizations drift toward universal access.

## Operational Uses

- Default-deny policies at all access control points.
- Role-based access with minimal permission sets.
- Just-in-time access elevation with time bounds.
- Access request workflows requiring business justification.
- Regular certification of existing access grants.

## Misuse / Abuse Risks

- Operational friction from overly restrictive defaults.
- Workarounds that bypass controls when access is too difficult.
- Over-reliance on approval workflows without actual review.
- Stale role definitions that no longer match job functions.

## Related Principles

- IDN-02.10 Attributable Identity
- IDN-02.11 Privilege Decay
- AUT-03.01 Authentication Boundary

## Compliance Touchpoints

Placeholder
