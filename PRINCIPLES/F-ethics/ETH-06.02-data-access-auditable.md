# ETH-06.02 — Data Access Auditable

## Statement

Data access must be auditable.

## Reasoning

Data protection requires knowing who accessed what data, when, and for
what purpose. Access without audit trails is access without
accountability. Auditability deters misuse, enables investigation of
breaches, and provides evidence for compliance.

Unaudited access is uncontrolled access.

## Justification

Data breaches often involve authorized users exceeding their intended
access scope. Without audit trails, organizations cannot detect
suspicious access patterns, cannot investigate after incidents, and
cannot demonstrate due diligence. Auditability transforms access
control from preventive to detective.

## Operational Uses

- Access logging for all sensitive data stores.
- Access pattern analysis and anomaly detection.
- Audit retention aligned to investigation needs.
- Regular access review using audit data.
- Forensic capability for access-related incidents.

## Misuse / Abuse Risks

- Audit volume creating storage and analysis challenges.
- Privacy concerns from detailed access tracking.
- Audit systems becoming attack targets.
- False confidence from incomplete audit coverage.

## Related Principles

- IDN-02.01 Attributable Identity
- ETH-06.01 Data Collection Justified
- IDN-02.07 Explainable Authorization

## Compliance Touchpoints

Placeholder
