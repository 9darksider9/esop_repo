# VIS-01.06 — Schema Drift Defect

## Statement

Schema drift is a production defect.

## Reasoning

Telemetry analysis depends on predictable structure. When schemas change
without coordination, parsers break, queries fail, dashboards show
incorrect data, and alerts stop firing. Schema drift degrades
observability as surely as collection failure.

Schema changes must be versioned, communicated, and coordinated with
downstream consumers. Unannounced changes are operational incidents.

## Justification

Detection rules written against specific field names and formats fail
silently when schemas change. Historical queries become unreliable.
Machine learning models trained on old schemas produce incorrect
predictions. Each uncontrolled schema change creates technical debt
in the observability stack.

## Operational Uses

- Schema registries with version control.
- Breaking change detection in CI/CD pipelines.
- Consumer notification for schema changes.
- Backward compatibility requirements for schema evolution.
- Schema validation at ingestion points.

## Misuse / Abuse Risks

- Schema rigidity preventing necessary evolution.
- Version proliferation creating management overhead.
- Backward compatibility constraints limiting improvements.
- False confidence from schema validation that misses semantic changes.

## Related Principles

- VIS-01.03 Telemetry Quality
- ENG-05.05 Drift Detection
- ENG-05.06 Configuration Is Code

## Compliance Touchpoints

Placeholder
