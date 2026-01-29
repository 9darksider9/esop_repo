# VIS-01.07 — Completeness Over Precision

## Statement

Missing data is more dangerous than noisy data.

## Reasoning

Noisy telemetry can be filtered, deduplicated, and normalized. Missing
telemetry cannot be recovered after the fact. Gaps in observability
create blind spots that attackers exploit and that investigators cannot
reconstruct.

Security analysis requires completeness before precision. A system that
drops events under load or fails silently provides false assurance.

## Justification

Incident investigations consistently fail when critical time windows
lack telemetry coverage. Missing logs, dropped events, collection gaps,
and failed forwarders create irrecoverable blind spots. Attackers
deliberately operate during collection outages or target logging
infrastructure to create gaps.

Noise can be addressed with better schemas, sampling strategies, and
filtering. Missing data requires time travel.

## Operational Uses

- Collection pipeline monitoring with gap detection.
- Alerting on telemetry source silence or volume anomalies.
- Backpressure handling that preserves data over throughput.
- Redundant collection paths for critical sources.
- Integrity validation of telemetry completeness.

## Misuse / Abuse Risks

- Tolerating excessive noise under the premise that completeness matters.
- Storage cost explosion without lifecycle management.
- Performance degradation from unbounded collection.
- Alert fatigue from low-value high-volume sources.

## Related Principles

- VIS-01.01 Telemetry Required
- VIS-01.04 Forensic Retention
- VIS-01.08 Collection Gaps Alert

## Compliance Touchpoints

Placeholder
