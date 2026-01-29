# P-080 Configuration as Code

## Statement

Configurations must be version-controlled and auditable; manual
configuration is exceptional.

## Reasoning

Manual configuration creates undocumented state that cannot be
reproduced, audited, or compared. Version-controlled configuration
provides history, enables review, supports rollback, and ensures
consistency across environments.

Exceptional manual changes must be documented and reconciled with
authoritative configuration sources.

## Justification

Configuration drift is a primary source of security incidents. Systems
manually configured diverge from baselines, accumulate ad-hoc changes,
and become irreproducible. Troubleshooting changes become permanent.
Security settings are disabled and never re-enabled.

Version-controlled configuration enables reconstruction after compromise,
consistency validation, and change attribution.

## Operational Uses

- Infrastructure as code for all environments.
- Configuration management with drift detection.
- Code review for configuration changes.
- Automated deployment from version control.
- Environment parity enforcement.

## Misuse / Abuse Risks

- Configuration code becoming as complex as application code.
- Secrets accidentally committed to version control.
- Drift between configuration code and actual state.
- Overhead for truly ephemeral or experimental systems.

## Related Principles

- P-020 Automation Default
- P-071 Rollback Capability
- P-081 Drift Detection

## Compliance Touchpoints

Placeholder
