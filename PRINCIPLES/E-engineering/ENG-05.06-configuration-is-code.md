# ENG-05.06 — Configuration Is Code

## Statement

Configuration is code.

## Reasoning

Configuration changes have the same impact as code changes: they alter
system behavior, can introduce vulnerabilities, and require the same
rigor. Treating configuration as less-than-code creates a control gap
where changes bypass review, testing, and version control.

Configuration deserves the same discipline as code.

## Justification

Many security incidents originate from configuration changes:
permissions broadened, encryption disabled, controls bypassed. When
configuration changes skip the controls applied to code changes, they
become a preferred path for both accidents and attacks.

## Operational Uses

- Version control for all configuration.
- Code review for configuration changes.
- Testing pipelines for configuration validation.
- Rollback capability for configuration changes.
- Audit trails for configuration history.

## Misuse / Abuse Risks

- Process overhead slowing necessary configuration changes.
- Configuration complexity matching code complexity.
- Secrets accidentally committed with configuration.
- Rigid processes preventing emergency changes.

## Related Principles

- ENG-05.05 Drift Detection
- ENG-05.07 Change Attribution
- AUT-03.04 Observable Automation

## Compliance Touchpoints

Placeholder
