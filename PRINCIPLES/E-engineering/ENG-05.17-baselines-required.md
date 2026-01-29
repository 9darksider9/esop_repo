# ENG-05.17 — Baselines Are Required

## Statement

Every system must have an explicit, versioned configuration baseline.

## Reasoning

Configuration baselines define the expected state of a system. Without an
explicit baseline, there is no reference point against which to detect
deviation, validate compliance, or restore known-good configurations.
Versioning enables tracking changes over time and rolling back to previous
states when necessary.

Implicit or undocumented configurations cannot be audited, reproduced, or
defended. What is not defined cannot be enforced.

## Justification

Systems without baselines drift unpredictably. Configuration inconsistencies
accumulate through manual changes, emergency fixes, and forgotten experiments.
Incident response teams cannot distinguish malicious changes from legitimate
ones without a reference point. Recovery requires rebuilding from scratch
rather than restoring to known-good state.

Explicit baselines convert configuration from tribal knowledge to auditable
artifacts.

## Operational Uses

- Version-controlled configuration repositories for all systems.
- Baseline snapshots captured before and after changes.
- Automated baseline generation from infrastructure-as-code.
- Baseline validation as deployment gate criteria.
- Baseline comparison during incident investigation.

## Misuse / Abuse Risks

- Baseline maintenance overhead for rapidly-changing systems.
- Stale baselines that no longer reflect operational requirements.
- Over-specification constraining legitimate operational flexibility.
- Baseline proliferation creating management complexity.

## Related Principles

- ENG-05.06 Configuration Is Code
- ENG-05.05 Drift Detection
- ENG-05.18 Drift Is a Security Signal

## Compliance Touchpoints

Placeholder
