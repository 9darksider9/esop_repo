# P-039 Recovery Exercised

## Statement

Recovery must be exercised, not assumed.

## Reasoning

Systems behave differently under failure than under design assumptions.
Documentation, runbooks, and theoretical recovery plans do not validate
real-world recoverability. Only exercised recovery demonstrates that
dependencies, credentials, data integrity, sequencing, and human
workflows function correctly under stress.

Assuming recoverability without validation creates latent systemic risk
and false confidence.

## Justification

Post-incident analysis consistently shows that recovery plans fail due
to stale documentation, missing credentials, undeclared dependencies,
broken backups, untested automation, or human coordination breakdowns.
Many organizations discover recovery defects only during real outages
or breaches, when time pressure amplifies impact.

Regular exercises surface hidden coupling, operational drift, and
tooling degradation before they become catastrophic.

## Operational Uses

- Scheduled disaster recovery exercises and tabletop simulations.
- Automated recovery testing in lower environments.
- Validation of backup integrity and restore timing.
- Verification of access paths required during emergencies.
- Measurement of recovery time and recovery point objectives.

## Misuse / Abuse Risks

- Performing superficial tests that do not reflect realistic failure.
- Treating exercise completion as compliance theater.
- Over-optimizing for test metrics rather than true resilience.
- Fatigue from excessive testing without automation.

## Related Principles

- P-035 Assume Compromise
- P-043 Recovery Objectives Validated
- P-054 Untestable Untrustworthy

## Compliance Touchpoints

Placeholder
