# ENG-05.14 — Change Validation

## Statement

Changes must be validated against security baselines before deployment.

## Reasoning

Changes that pass functional testing may still introduce security
regressions. Validation against security baselines catches configuration
errors, permission changes, and policy violations before they reach
production. Post-deployment discovery of security issues is more
expensive and risky.

Automated validation enables security gates without becoming bottlenecks.

## Justification

Security regressions frequently enter production through changes that
were not evaluated for security impact: default password reintroduced,
encryption disabled for troubleshooting, permissions broadened for
convenience. These changes pass functional testing because they do not
break features.

Pre-deployment security validation catches what functional testing
misses.

## Operational Uses

- Security policy checks in CI/CD pipelines.
- Infrastructure as code security scanning.
- Configuration drift detection before deployment.
- Credential and secret scanning.
- Compliance validation gates.

## Misuse / Abuse Risks

- False positives blocking legitimate deployments.
- Validation becoming bottleneck if not automated.
- Incomplete baselines missing important checks.
- Developers bypassing validation through exceptions.

## Related Principles

- ENG-05.07 Testability
- ENG-05.10 Change Authorization
- ENG-05.15 Baseline Enforcement

## Compliance Touchpoints

Placeholder
