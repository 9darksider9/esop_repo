# AUT-03.04 — Observable Automation

## Statement

Automation must be observable, reversible, and bounded.

## Reasoning

Automation that cannot be observed cannot be trusted. Automation that
cannot be reversed cannot be safely deployed. Automation without bounds
can cause unbounded damage. These properties—observability,
reversibility, boundedness—are prerequisites for safe automation.

Uncontrolled automation is not an improvement over uncontrolled manual
work.

## Justification

Automation failures at scale can cause cascading damage that exceeds
the cost of manual errors. Without observability, failures go undetected.
Without reversibility, failures cannot be corrected. Without bounds,
failures cannot be contained. Each property is necessary for automation
that improves rather than amplifies risk.

## Operational Uses

- Comprehensive logging for all automation actions.
- Rollback capabilities for automated changes.
- Rate limits and scope constraints on automation.
- Circuit breakers that halt runaway automation.
- Dry-run modes for testing automation safely.

## Misuse / Abuse Risks

- Observability overhead affecting automation performance.
- Reversibility constraints limiting automation scope.
- Bounds set too conservatively limiting automation value.
- False confidence from incomplete observability.

## Related Principles

- AUT-03.02 Intent and Execution Separation
- AUT-03.06 Automation Failure Safety
- RES-04.07 Containment Automatable

## Compliance Touchpoints

Placeholder
