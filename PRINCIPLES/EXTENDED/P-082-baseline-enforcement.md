# P-082 Baseline Enforcement

## Statement

Systems must conform to approved security baselines; deviations require
documented exceptions.

## Reasoning

Security baselines encode organizational security requirements into
verifiable configurations. Baseline enforcement ensures that all systems
meet minimum security standards. Exceptions document accepted risk and
enable periodic review.

Uncontrolled deviation from baselines creates inconsistent security
posture and unknown risk.

## Justification

Organizations with inconsistent configurations cannot make reliable
security claims. Each deviation represents potential exposure.
Vulnerability remediation becomes complex when systems differ.
Incident response is complicated by unknown configurations.

Baselines also enable automation: systems that conform to baselines
can be managed uniformly.

## Operational Uses

- Hardening standards encoded as verifiable policies.
- Automated compliance scanning against baselines.
- Exception workflows with documented justification.
- Baseline updates through governed change processes.
- Tiered baselines for different risk classifications.

## Misuse / Abuse Risks

- Baselines becoming stale as threats evolve.
- Excessive exceptions undermining baseline value.
- One-size-fits-all baselines ignoring legitimate variation.
- Compliance focus on baseline rather than actual security.

## Related Principles

- P-042 Secure Defaults
- P-072 Change Validation
- P-081 Drift Detection

## Compliance Touchpoints

Placeholder
