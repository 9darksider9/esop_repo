# RES-04.13 — Vulnerabilities Are Contextual

## Statement

Vulnerabilities must be evaluated in the context of exposure, reachability,
and compensating controls.

## Reasoning

Raw vulnerability severity scores do not reflect actual risk. A critical
vulnerability on an isolated, unexposed system presents less immediate risk
than a medium vulnerability on an internet-facing asset with no compensating
controls. Context determines exploitability; exploitability determines
priority.

Treating all vulnerabilities equally wastes remediation resources and fails
to address actual risk.

## Justification

Organizations that prioritize purely by CVSS score remediate vulnerabilities
that attackers cannot reach while leaving exploitable weaknesses unaddressed.
Security teams become overwhelmed by volume while actual attack surface
remains exposed.

Contextual evaluation focuses remediation effort where it reduces real risk.

## Operational Uses

- Asset exposure mapping for vulnerability prioritization.
- Reachability analysis from untrusted networks to vulnerable systems.
- Compensating control inventory against specific vulnerabilities.
- Risk-adjusted vulnerability scores incorporating environmental factors.
- Exploit availability as prioritization factor.

## Misuse / Abuse Risks

- Context assessment overhead delaying remediation.
- Incorrect exposure assumptions leaving vulnerabilities unaddressed.
- Compensating controls used to justify indefinite deferral.
- Complexity enabling rationalization of inaction.

## Related Principles

- RES-04.02 Blast Radius Measurable
- ENG-05.19 Unmanaged Vulnerabilities Are Defects
- ENG-05.03 Evidence Over Opinion

## Compliance Touchpoints

Placeholder
