# VIS-01.11 — Observable Decisions

## Statement

Every security decision must reference observable data.

## Reasoning

Security decisions based on assumptions, intuition, or stale information
cannot be validated, audited, or improved. Observable data provides the
foundation for defensible decisions, continuous learning, and
accountability.

Decisions without data are opinions. Opinions do not scale and cannot
be systematically improved.

## Justification

Post-incident reviews frequently reveal that decisions were made without
consulting available data, or that required data was not available.
Decision quality improves when decisions are grounded in observation
rather than assumption. Audit and compliance require demonstrable basis
for security conclusions.

## Operational Uses

- Decision logging with data references.
- Required data fields in security workflows.
- Automated decision support from telemetry.
- Decision audit trails linking conclusions to evidence.
- Metrics on data-driven versus assumption-driven decisions.

## Misuse / Abuse Risks

- Analysis paralysis waiting for perfect data.
- Over-reliance on available data when critical data is missing.
- Data manipulation to support predetermined conclusions.
- Decision latency from data retrieval requirements.

## Related Principles

- ENG-05.03 Evidence Over Opinion
- VIS-01.05 Data Lineage
- IDN-02.07 Explainable Authorization

## Compliance Touchpoints

Placeholder
