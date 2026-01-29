# P-002 Telemetry Implies Trust

## Statement

Assets without telemetry are considered compromised until proven
otherwise.

## Reasoning

The absence of telemetry is indistinguishable from successful attacker
suppression of telemetry. An asset that produces no observable data
cannot be validated as secure, cannot be monitored for compromise, and
cannot be investigated. The conservative security assumption treats
silence as evidence of compromise rather than evidence of health.

Trust requires continuous proof. Systems that cannot demonstrate their
state through telemetry have not earned operational trust.

## Justification

Attackers prioritize disabling logging and evading detection. Silent
assets may be functioning correctly or may be fully compromised with
telemetry suppressed. Organizations cannot distinguish between these
states without observable data.

Treating telemetry gaps as security events forces rapid remediation
and prevents attackers from exploiting monitoring blind spots.

## Operational Uses

- Telemetry heartbeat monitoring with silence alerts.
- Automatic quarantine of assets that stop producing telemetry.
- Risk scoring that penalizes assets with telemetry gaps.
- Incident triggers when expected telemetry sources go silent.
- Asset health dashboards showing telemetry coverage.

## Misuse / Abuse Risks

- False positives from legitimate maintenance windows.
- Over-aggressive quarantine disrupting operations.
- Alert fatigue from transient network issues.
- Difficulty distinguishing collection failures from source failures.

## Related Principles

- P-001 Telemetry Required
- P-008 Collection Gaps Alert
- P-044 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
