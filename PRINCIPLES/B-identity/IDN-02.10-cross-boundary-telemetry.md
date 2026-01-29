# IDN-02.10 — Cross-Boundary Telemetry

## Statement

Cross-boundary access requires compensating telemetry.

## Reasoning

Access across trust boundaries represents elevated risk. When access
crosses a boundary, visibility requirements increase correspondingly.
Compensating telemetry ensures that boundary crossings are observable,
attributable, and analyzable even when boundary controls are bypassed.

More access requires more observation.

## Justification

Lateral movement attacks exploit boundary crossings that lack
sufficient monitoring. If an attacker can cross boundaries without
generating distinctive telemetry, detection depends entirely on
boundary controls. Compensating telemetry provides defense in depth
for boundary violations.

## Operational Uses

- Enhanced logging for cross-boundary operations.
- Step-up authentication at boundary crossings.
- Correlation rules for multi-boundary access patterns.
- Behavioral baselines for cross-boundary activity.
- Alerting on anomalous boundary crossing patterns.

## Misuse / Abuse Risks

- Telemetry overhead slowing cross-boundary operations.
- Log volume explosion from high-frequency crossings.
- False positives from legitimate cross-boundary patterns.
- Inconsistent boundary definitions across telemetry sources.

## Related Principles

- IDN-02.09 Explicit Trust Boundaries
- VIS-01.01 Telemetry Required
- RES-04.03 Lateral Movement Visible

## Compliance Touchpoints

Placeholder
