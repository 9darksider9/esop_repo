# VIS-01.08 — Collection Gaps Alert

## Statement

Collection gaps must trigger alerts.

## Reasoning

Telemetry collection is not self-evidently reliable. Forwarders fail,
networks partition, buffers overflow, and configurations drift. Without
active monitoring for collection health, gaps accumulate silently until
an incident reveals the blind spot.

Collection gaps are security events, not operational inconveniences.
They must be detected and remediated with the same urgency as
production outages.

## Justification

Organizations routinely discover during investigations that critical
telemetry was not being collected for days, weeks, or months. These
gaps are often caused by silent failures in collection infrastructure
that went unmonitored. Attackers time operations to coincide with
collection outages or actively induce them.

## Operational Uses

- Heartbeat monitoring for all telemetry sources.
- Volume anomaly detection for collection pipelines.
- Expected-versus-actual source reconciliation.
- Collection health dashboards with SLA tracking.
- Automated alerting on gap detection.

## Misuse / Abuse Risks

- Alert fatigue from transient collection issues.
- False positives during maintenance windows.
- Difficulty distinguishing source failures from pipeline failures.
- Over-reliance on volume metrics missing content gaps.

## Related Principles

- VIS-01.02 Telemetry Implies Trust
- VIS-01.07 Completeness Over Precision
- RES-04.10 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
