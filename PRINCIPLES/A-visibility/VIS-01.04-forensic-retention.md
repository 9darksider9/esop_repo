# VIS-01.04 — Forensic Retention

## Statement

Raw telemetry must be preserved long enough to support forensic
reconstruction.

## Reasoning

Security investigations often begin weeks or months after initial
compromise. If raw telemetry has been deleted or aged out, forensic
reconstruction becomes impossible. Derived data and aggregations lose
the detail needed to answer investigative questions.

Retention periods must account for typical dwell times, regulatory
requirements, and investigation timelines—not just storage costs.

## Justification

Advanced persistent threats maintain access for extended periods before
detection. Post-breach investigations require reconstructing attacker
activity across the full dwell time. Organizations that delete raw
telemetry before detection occurs cannot determine scope, root cause,
or complete remediation.

Derived data cannot substitute for raw events when novel questions arise.

## Operational Uses

- Retention policies aligned to threat dwell time statistics.
- Tiered storage for cost-effective long-term retention.
- Immutable storage for forensically critical sources.
- Retention validation ensuring data is actually preserved.
- Legal hold procedures for investigation-relevant data.

## Misuse / Abuse Risks

- Storage cost explosion without lifecycle management.
- Privacy exposure from excessive retention.
- Performance degradation from querying aged data.
- Regulatory conflicts between retention and deletion requirements.

## Related Principles

- VIS-01.05 Data Lineage
- VIS-01.07 Completeness Over Precision
- VIS-01.03 Telemetry Quality

## Compliance Touchpoints

Placeholder
