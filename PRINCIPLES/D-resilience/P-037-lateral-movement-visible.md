# P-037 Lateral Movement Visible

## Statement

Lateral movement paths must be visible.

## Reasoning

Attackers who gain initial access seek to expand their foothold through
lateral movement. If lateral movement paths are not visible, defenders
cannot identify how attackers might pivot, cannot detect movement in
progress, and cannot contain breaches effectively.

Visibility precedes control. You cannot block paths you cannot see.

## Justification

Major breaches consistently feature undetected lateral movement through
trust relationships, shared credentials, and network adjacency.
Organizations that cannot visualize lateral movement paths discover
them only during incident response, when containment is already
compromised.

## Operational Uses

- Network topology mapping including trust relationships.
- Credential usage monitoring across systems.
- Authentication pattern analysis for anomalous pivots.
- Attack path modeling and analysis.
- Segmentation effectiveness validation.

## Misuse / Abuse Risks

- Visibility complexity in large environments.
- False confidence from incomplete path mapping.
- Analysis paralysis from too many visible paths.
- Visibility tools becoming attack targets.

## Related Principles

- P-021 Explicit Trust Boundaries
- P-036 Blast Radius Measurable
- P-022 Cross-Boundary Telemetry

## Compliance Touchpoints

Placeholder
