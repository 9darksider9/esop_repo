# P-070 Change Authorization

## Statement

Changes require documented authorization before implementation;
unauthorized changes are incidents.

## Reasoning

Uncontrolled changes introduce unpredictable risk. Authorization ensures
that changes are reviewed for security impact, tested appropriately, and
traceable to accountable parties. Unauthorized changes cannot be
distinguished from attacker activity.

Documentation provides audit trail for compliance, troubleshooting, and
incident investigation.

## Justification

Many security incidents originate from unauthorized or poorly reviewed
changes: configuration errors, deployment mistakes, and undocumented
modifications. Attackers disguise malicious changes as routine
operations. Without authorization controls, legitimate and malicious
changes are indistinguishable.

Change control also enables rollback by establishing known-good states.

## Operational Uses

- Change request and approval workflows.
- Automated enforcement of authorization in deployment pipelines.
- Detection of unauthorized modifications.
- Separation of duties between requesters and approvers.
- Emergency change procedures with post-hoc review.

## Misuse / Abuse Risks

- Process overhead slowing critical security responses.
- Rubber-stamp approvals that do not provide actual review.
- Workarounds that bypass controls for convenience.
- Overly rigid processes that cannot accommodate emergencies.

## Related Principles

- P-020 Automation Default
- P-071 Rollback Capability
- P-072 Change Validation

## Compliance Touchpoints

Placeholder
