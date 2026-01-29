# AUT-03.08 — Complexity Compounds Risk

## Statement

Operational complexity compounds risk faster than technical complexity.

## Reasoning

Complex operations—handoffs, coordination, dependencies, exceptions—
create opportunities for error, miscommunication, and oversight.
Operational complexity compounds across every execution, while
technical complexity is contained within systems. The more complex
the operation, the more likely it fails under pressure.

Simplicity is a security property.

## Justification

Incident post-mortems consistently reveal that operational complexity
contributed to failure: unclear handoffs, missed steps, exception
handling errors, and coordination failures. Technical systems can be
tested; operational complexity often cannot. Reducing operational
complexity reduces the attack surface that emerges from human factors.

## Operational Uses

- Operational complexity as an architecture review criterion.
- Runbook simplification as a security improvement.
- Handoff elimination where possible.
- Exception reduction through better defaults.
- Complexity metrics for operational processes.

## Misuse / Abuse Risks

- Oversimplifying operations that require nuance.
- Technical complexity hidden by simple operational facades.
- Simplicity goals conflicting with necessary controls.
- Ignoring necessary operational safeguards.

## Related Principles

- AUT-03.09 Reliability Over Cleverness
- AUT-03.07 Human Toil Signal
- ENG-05.09 Security Debt Compounds

## Compliance Touchpoints

Placeholder
