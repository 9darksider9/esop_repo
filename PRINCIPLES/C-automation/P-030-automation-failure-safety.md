# P-030 Automation Failure Safety

## Statement

Automation failure must degrade safely.

## Reasoning

Automation will fail. Networks partition, dependencies become
unavailable, and edge cases trigger unexpected behavior. When
automation fails, the failure mode must be predictable, contained,
and safe rather than unpredictable, cascading, or dangerous.

Fail-safe automation preserves security posture during failures
rather than degrading it.

## Justification

Automation failures that bypass security controls, grant expanded
access, or cause cascading damage are worse than no automation.
Attackers may deliberately trigger automation failures to exploit
unsafe failure modes. Safe degradation ensures that failures do not
become security incidents.

## Operational Uses

- Fail-closed defaults for security automation.
- Graceful degradation paths for automation dependencies.
- Circuit breakers halting failed automation.
- Fallback procedures when automation is unavailable.
- Failure mode testing for all critical automation.

## Misuse / Abuse Risks

- Fail-closed causing availability incidents.
- Fallback procedures creating shadow manual operations.
- Degradation paths not tested regularly.
- Over-engineering failure handling for unlikely scenarios.

## Related Principles

- P-028 Observable Automation
- P-020 Identity Resilience
- P-044 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
