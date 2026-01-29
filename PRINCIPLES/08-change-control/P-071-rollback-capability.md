# P-071 Rollback Capability

## Statement

Changes must be reversible or have documented recovery procedures;
irreversible changes require additional scrutiny.

## Reasoning

Changes fail. Unexpected interactions cause problems. Rollback capability
enables rapid recovery from failed changes without requiring forward-fix
under pressure. Irreversible changes commit the organization to outcomes
that cannot be undone if problems emerge.

Reversibility reduces risk by enabling experimentation and rapid
iteration with manageable consequences.

## Justification

Organizations that cannot roll back changes must fix forward during
outages and security incidents, increasing time to recovery and
introducing additional risk under pressure. Many incidents escalate
because initial remediation attempts create new problems that cannot
be undone.

Irreversible changes should be rare, well-documented, and subject to
enhanced review.

## Operational Uses

- Version control for all configuration and code.
- Database migration reversibility requirements.
- Deployment strategies supporting instant rollback.
- Backup verification before destructive operations.
- Documented recovery procedures for irreversible changes.

## Misuse / Abuse Risks

- Relying on rollback instead of proper pre-deployment testing.
- Incomplete rollback that leaves systems in inconsistent states.
- Data loss during rollback of stateful changes.
- Complexity from maintaining rollback capability for all changes.

## Related Principles

- P-021 Idempotent Operations
- P-070 Change Authorization
- P-080 Configuration as Code

## Compliance Touchpoints

Placeholder
