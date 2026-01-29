# P-005 Data Lineage

## Statement

Derived data must always be traceable back to original source events.

## Reasoning

Security decisions based on derived data—aggregations, alerts,
metrics, scores—require validation against source events. If lineage
is broken, derived data cannot be verified, false positives cannot be
investigated, and audit requirements cannot be satisfied.

Traceability ensures that conclusions can be validated and that
processing errors can be identified and corrected.

## Justification

Alert fatigue often stems from inability to validate derived signals
against source data. Compliance audits require demonstrating how
conclusions were reached. Incident investigations require drilling
from alerts to raw events. Without lineage, derived data is opinion.

## Operational Uses

- Correlation identifiers linking derived data to source events.
- Drill-down capabilities from dashboards to raw logs.
- Audit trails for data transformations.
- Validation pipelines comparing derived and source data.
- Documentation of aggregation and enrichment logic.

## Misuse / Abuse Risks

- Lineage metadata overhead affecting performance.
- Complexity in multi-stage processing pipelines.
- Storage costs for maintaining source references.
- Lineage becoming stale when pipelines change.

## Related Principles

- P-004 Forensic Retention
- P-047 Evidence Over Opinion
- P-011 Observable Decisions

## Compliance Touchpoints

Placeholder
