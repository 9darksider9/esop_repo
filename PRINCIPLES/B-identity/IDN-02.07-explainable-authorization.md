# IDN-02.07 — Explainable Authorization

## Statement

Authorization decisions must be explainable post-fact.

## Reasoning

When access is granted or denied, the reasoning must be reconstructible.
Opaque authorization—where decisions cannot be explained—resists audit,
prevents troubleshooting, and obscures policy errors. If you cannot
explain why access was granted, you cannot verify it was correct.

Explainability enables accountability, debugging, and continuous
improvement of authorization logic.

## Justification

Incident investigations frequently need to determine how an attacker
obtained access. Compliance audits require demonstrating authorization
correctness. Operational troubleshooting requires understanding why
legitimate access was denied. All these needs require explainable
authorization decisions.

## Operational Uses

- Authorization decision logging with policy references.
- Debug modes that explain evaluation paths.
- Policy simulation tools for testing access decisions.
- Audit reporting of authorization rationale.
- Root cause analysis for access-related incidents.

## Misuse / Abuse Risks

- Verbose logging creating performance or storage overhead.
- Explanation complexity obscuring simple decisions.
- Security through obscurity arguments against transparency.
- Gaming of authorization logic when evaluation is visible.

## Related Principles

- VIS-01.11 Observable Decisions
- IDN-02.01 Attributable Identity
- ENG-05.03 Evidence Over Opinion

## Compliance Touchpoints

Placeholder
