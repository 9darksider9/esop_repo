# VIS-01.10 — Data Freshness

## Statement

Data freshness must be measurable and enforced.

## Reasoning

Stale data drives incorrect decisions. Security controls that rely on
data from minutes, hours, or days ago operate on fiction, not reality.
Freshness requirements must be explicit, measured, and enforced—not
assumed.

Different use cases have different freshness tolerances, but all
tolerances must be defined and validated.

## Justification

Real-time detection systems fed by batch pipelines miss active attacks.
Access decisions based on stale identity data permit revoked access.
Dashboards showing outdated metrics create false confidence. Without
freshness measurement, staleness accumulates silently.

## Operational Uses

- Freshness SLAs for each telemetry source.
- Latency monitoring in collection pipelines.
- Staleness alerts when freshness exceeds thresholds.
- Timestamp validation at consumption points.
- Freshness metadata in derived data.

## Misuse / Abuse Risks

- Overly aggressive freshness requirements increasing infrastructure
  costs.
- Freshness alerts creating noise without actionable remediation.
- Clock skew causing false staleness detection.
- Freshness optimization displacing completeness optimization.

## Related Principles

- VIS-01.03 Telemetry Quality
- VIS-01.11 Observable Decisions
- VIS-01.08 Collection Gaps Alert

## Compliance Touchpoints

Placeholder
