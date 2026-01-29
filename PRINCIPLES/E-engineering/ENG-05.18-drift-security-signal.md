# ENG-05.18 — Drift Is a Security Signal

## Statement

Deviation from approved configuration baselines is a security-relevant event.

## Reasoning

Configuration drift indicates that reality no longer matches intent. Whether
caused by unauthorized changes, malicious activity, or operational error,
drift must be treated as security-relevant until its cause is understood.
Attackers modify configurations to persist access, disable controls, and
enable lateral movement.

Drift that is ignored becomes normalized. Normalized drift erodes the
integrity of the entire configuration management system.

## Justification

Attackers routinely modify configurations during intrusions: disabling
logging, adding user accounts, opening firewall ports, installing persistence
mechanisms. Organizations that do not monitor for drift cannot distinguish
attacker modifications from operational changes.

Drift detection provides early warning of compromise and validates that
security controls remain in their intended state.

## Operational Uses

- Real-time drift detection against approved baselines.
- Drift alerts routed to security operations for triage.
- Automated remediation of unauthorized configuration changes.
- Drift investigation as standard incident response procedure.
- Drift metrics as security posture indicators.

## Misuse / Abuse Risks

- Alert fatigue from excessive drift notifications.
- False positives from legitimate but undocumented changes.
- Remediation automation causing operational disruption.
- Drift tolerance exceptions that become permanent.

## Related Principles

- ENG-05.17 Baselines Are Required
- ENG-05.05 Drift Detection
- ENG-05.07 Change Attribution

## Compliance Touchpoints

Placeholder
