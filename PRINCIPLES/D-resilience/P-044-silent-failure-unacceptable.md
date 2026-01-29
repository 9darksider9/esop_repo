# P-044 Silent Failure Unacceptable

## Statement

Silent failure is unacceptable.

## Reasoning

Systems that fail without notification leave defenders operating with
false assumptions. Silent failures allow attacks to proceed undetected,
allow controls to degrade without awareness, and create false
confidence in security posture. Every failure must produce a signal.

Unknown failures are worse than known failures.

## Justification

Many breaches persist because security controls failed silently.
Detection systems stopped working, collection pipelines broke, and
monitoring tools crashed—all without alerting anyone. Silent failure
is a gift to attackers who benefit from defender ignorance.

## Operational Uses

- Health checks for all security systems.
- Alerting on system silence, not just system errors.
- Dead-man switches for critical controls.
- Heartbeat monitoring for security infrastructure.
- Failure notification as a first-class requirement.

## Misuse / Abuse Risks

- Alert fatigue from excessive failure notifications.
- Noise from transient failures.
- False positives masking real failures.
- Notification overhead affecting system performance.

## Related Principles

- P-002 Telemetry Implies Trust
- P-008 Collection Gaps Alert
- P-030 Automation Failure Safety

## Compliance Touchpoints

Placeholder
