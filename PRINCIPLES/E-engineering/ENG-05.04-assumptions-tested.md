# ENG-05.04 — Assumptions Tested

## Statement

Assumptions must be documented and tested.

## Reasoning

Security architectures rest on assumptions—about threats, behaviors,
capabilities, and constraints. Undocumented assumptions cannot be
evaluated. Untested assumptions may be invalid. When assumptions fail,
security fails. Making assumptions explicit enables validation and
early detection of invalid assumptions.

Hidden assumptions are hidden vulnerabilities.

## Justification

Post-incident analysis frequently reveals that security designs failed
because underlying assumptions were invalid. "We assumed the firewall
would block that traffic." "We assumed users wouldn't share
credentials." Explicit documentation and testing of assumptions
surfaces these vulnerabilities before incidents.

## Operational Uses

- Assumption documentation in architecture artifacts.
- Assumption testing in security reviews.
- Assumption monitoring for environmental changes.
- Threat model updates when assumptions change.
- Regular assumption validity reviews.

## Misuse / Abuse Risks

- Assumption documentation becoming pro-forma.
- Testing overhead for stable assumptions.
- Paralysis from uncertainty about assumptions.
- Missing emergent assumptions not in documentation.

## Related Principles

- ENG-05.03 Evidence Over Opinion
- ENG-05.10 Untestable Untrustworthy
- RES-04.05 Recovery Exercised

## Compliance Touchpoints

Placeholder
