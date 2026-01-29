# P-022 Audit Trail Mandatory

## Statement

Automated actions must produce immutable, attributable audit records.

## Reasoning

Automation operates at machine speed across many systems. Without
comprehensive audit trails, automated actions cannot be investigated,
validated, or reversed. Security depends on the ability to reconstruct
what happened, when, and under what authority.

Audit records must be immutable to prevent post-hoc modification and
attributable to identify the automation, its trigger, and its authority.

## Justification

Automated remediation that lacks audit trails creates accountability
gaps. Security teams cannot distinguish between authorized automation
and attacker actions. Compliance cannot validate that controls operated
correctly. Incident response cannot reconstruct timelines.

Attackers exploit automation systems specifically because they often
lack the scrutiny applied to interactive access.

## Operational Uses

- Structured logging from all automation frameworks.
- Correlation identifiers linking triggers to actions.
- Capture of inputs, outputs, and state changes.
- Retention policies aligned to investigation needs.
- Separation of audit storage from automation systems.

## Misuse / Abuse Risks

- Verbose logging creating performance or cost problems.
- Sensitive data exposure in audit records.
- Audit systems becoming attack targets.
- Log volume obscuring significant events.

## Related Principles

- P-001 Telemetry Required
- P-003 Telemetry Integrity
- P-020 Automation Default

## Compliance Touchpoints

Placeholder
