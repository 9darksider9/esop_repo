# ENG-05.08 — Repeat Failures Systemic

## Statement

Repeat failures indicate systemic defects.

## Reasoning

When the same failure occurs multiple times, the root cause is not the
immediate trigger but the system that allows the failure to recur.
Treating repeat failures as isolated incidents guarantees continued
failure. Systemic defects require systemic remediation.

Repeat failures are architecture signals, not operator errors.

## Justification

Organizations often respond to repeat failures with workarounds,
training, or admonishment rather than architectural fixes. These
responses do not prevent recurrence. Treating repeat failures as
systemic defects forces investment in root cause remediation rather
than symptom treatment.

## Operational Uses

- Failure pattern tracking and correlation.
- Root cause analysis for recurring incidents.
- Architectural reviews triggered by repeat failures.
- Blameless postmortems focused on system improvement.
- Investment prioritization toward recurring failure elimination.

## Misuse / Abuse Risks

- Labeling single failures as systemic to avoid individual accountability.
- Analysis paralysis seeking systemic causes for random failures.
- Over-engineering solutions for infrequent failures.
- Ignoring genuine human factors in systemic analysis.

## Related Principles

- AUT-03.07 Human Toil Signal
- ENG-05.09 Security Debt Compounds
- ETH-06.07 Non-Punitive Telemetry

## Compliance Touchpoints

Placeholder
