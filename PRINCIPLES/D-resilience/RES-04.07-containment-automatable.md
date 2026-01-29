# RES-04.07 — Containment Automatable

## Statement

Containment must be automatable.

## Reasoning

When a breach is detected, containment speed determines damage scope.
Manual containment is too slow for modern attack velocity. Containment
actions—network isolation, credential revocation, system quarantine—
must be automatable and executable within seconds of detection.

Containment that requires human execution has already failed.

## Justification

Attackers automate their operations; defenders must automate theirs.
The window between detection and attacker persistence establishment
is measured in minutes. Manual containment workflows measured in hours
guarantee that containment arrives after persistence is established.

## Operational Uses

- Pre-authorized containment playbooks.
- Automated network isolation capabilities.
- Credential revocation automation.
- System quarantine automation.
- Containment testing in regular exercises.

## Misuse / Abuse Risks

- Automated containment causing false-positive disruption.
- Containment automation becoming attack vector.
- Over-broad containment scope affecting production.
- Containment automation bypassing change control.

## Related Principles

- AUT-03.02 Intent and Execution Separation
- RES-04.06 Detection Over Prevention
- AUT-03.04 Observable Automation

## Compliance Touchpoints

Placeholder
