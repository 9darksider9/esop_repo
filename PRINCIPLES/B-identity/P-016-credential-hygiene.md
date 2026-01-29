# P-016 Credential Hygiene

## Statement

Credentials must be short-lived, rotated automatically, and scoped
narrowly.

## Reasoning

Long-lived credentials provide extended windows for compromise.
Manual rotation is unreliable and creates operational gaps. Broadly
scoped credentials enable lateral movement when compromised.

Credential hygiene—short lifetimes, automatic rotation, narrow
scope—limits exposure from any single credential compromise.

## Justification

Most credential-based attacks exploit stale credentials, leaked
secrets, or over-privileged access. Reducing credential lifetime
reduces the window of opportunity. Automatic rotation eliminates
human error. Narrow scope limits blast radius.

## Operational Uses

- Token lifetime policies measured in hours, not days.
- Automated rotation for all machine credentials.
- Just-in-time credential issuance where possible.
- Scope validation during credential provisioning.
- Secret scanning and leak detection.

## Misuse / Abuse Risks

- Short lifetimes causing authentication failures.
- Rotation overhead in legacy systems.
- Narrow scope requiring frequent access requests.
- Automation complexity for rotation workflows.

## Related Principles

- P-015 Machine Identity Risk
- P-017 Standing Privilege Debt
- P-024 Workload-Based Privilege

## Compliance Touchpoints

Placeholder
