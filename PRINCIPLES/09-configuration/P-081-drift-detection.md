# P-081 Drift Detection

## Statement

Configuration drift must be detected and remediated; undetected drift
is assumed compromise.

## Reasoning

Production systems change. Troubleshooting modifications, emergency
fixes, and unauthorized changes accumulate. Without drift detection,
actual configuration diverges from intended configuration, creating
unknown security state.

Drift may be benign or may indicate compromise. Without detection,
the organization cannot distinguish between the two.

## Justification

Attackers modify configurations to establish persistence, disable
controls, and enable access. These changes blend with legitimate drift
if not detected. Organizations that do not detect drift cannot identify
unauthorized modifications.

Drift also indicates control failures: changes that bypassed review,
automation that failed, or policies that were not enforced.

## Operational Uses

- Continuous comparison of actual vs. intended state.
- Automated alerting on configuration changes.
- Reconciliation workflows for detected drift.
- Forensic baselines for incident investigation.
- Compliance evidence of configuration integrity.

## Misuse / Abuse Risks

- Alert fatigue from excessive drift notifications.
- Remediation automation causing unintended disruption.
- Legitimate operational drift incorrectly flagged.
- Performance overhead from continuous monitoring.

## Related Principles

- P-080 Configuration as Code
- P-082 Baseline Enforcement
- P-022 Audit Trail Mandatory

## Compliance Touchpoints

Placeholder
