# P-013 Attributable Identity

## Statement

Every action must have an attributable identity.

## Reasoning

Security accountability requires knowing who or what performed each
action. Shared accounts, anonymous access, and unattributed automation
create gaps where responsibility cannot be assigned and behavior cannot
be investigated.

Attribution enables access control enforcement, anomaly detection,
incident investigation, and accountability. Without attribution, security
controls operate blindly.

## Justification

Investigations stall when actions cannot be traced to specific actors.
Shared credentials prevent distinguishing between legitimate users and
compromised access. Service accounts without clear ownership become
orphaned attack vectors. Anonymous actions cannot be correlated with
behavioral patterns.

Attackers exploit attribution gaps to operate without detection and to
frustrate forensic analysis.

## Operational Uses

- Elimination of shared credentials and generic accounts.
- Service account ownership registration and lifecycle management.
- Machine identity issuance for automated systems.
- Session binding that maintains attribution across operations.
- Audit trail correlation by identity.

## Misuse / Abuse Risks

- Privacy overreach through excessive identity tracking.
- Friction from identity requirements in low-risk contexts.
- Identity sprawl from over-provisioning unique credentials.
- Attribution used for blame rather than learning.

## Related Principles

- P-014 Anonymous Access Defect
- P-018 Privilege Decay
- P-051 Change Attribution

## Compliance Touchpoints

Placeholder
