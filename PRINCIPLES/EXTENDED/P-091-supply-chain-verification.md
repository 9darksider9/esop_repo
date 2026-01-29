# P-091 Supply Chain Verification

## Statement

External dependencies must be verified and continuously monitored;
unverified dependencies are untrusted.

## Reasoning

Modern systems depend on external code, services, and infrastructure.
Each dependency represents a trust relationship. Compromised dependencies
propagate through all consuming systems. Verification ensures that
dependencies are authentic and monitored for compromise.

Supply chain attacks target dependencies specifically because they
provide leverage across many victims.

## Justification

High-profile supply chain attacks have compromised widely-used
libraries, build systems, and distribution channels. Organizations
that do not verify dependencies cannot detect when trusted components
become malicious.

Continuous monitoring catches newly-discovered vulnerabilities and
compromises in existing dependencies.

## Operational Uses

- Software composition analysis for all code dependencies.
- Integrity verification of downloaded packages.
- Vulnerability monitoring for dependency components.
- Approved dependency sources and registries.
- Dependency update policies and automation.

## Misuse / Abuse Risks

- Analysis overhead slowing development velocity.
- False positives from vulnerability scanners.
- Blocking critical updates due to verification delays.
- Incomplete coverage of non-code dependencies.

## Related Principles

- P-062 Dependency Tracking
- P-090 Vendor Assessment
- P-003 Telemetry Integrity

## Compliance Touchpoints

Placeholder
