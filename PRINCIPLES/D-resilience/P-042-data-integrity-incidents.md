# P-042 Data Integrity Incidents

## Statement

Data integrity failures are security incidents.

## Reasoning

Data integrity—the assurance that data has not been improperly
modified—is a security property. Integrity failures may indicate
attacker manipulation, insider threat, or control failures. Treating
integrity failures as operational issues rather than security incidents
allows attacks to proceed undetected.

Integrity violations must trigger security investigation.

## Justification

Attackers manipulate data to cover tracks, falsify records, and
undermine trust in systems. Integrity failures that are dismissed as
bugs or glitches may actually be attack indicators. Security rigor
requires treating integrity failures with the same seriousness as
confidentiality or availability failures.

## Operational Uses

- Integrity monitoring for critical data stores.
- Security alerting on integrity anomalies.
- Incident response procedures for integrity failures.
- Forensic investigation of integrity violations.
- Root cause analysis distinguishing attack from error.

## Misuse / Abuse Risks

- Alert fatigue from non-security integrity issues.
- Over-investigation of benign data inconsistencies.
- Resources diverted from other security priorities.
- Difficulty distinguishing malicious from accidental integrity loss.

## Related Principles

- P-003 Telemetry Quality
- P-040 Detection Over Prevention
- P-044 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
