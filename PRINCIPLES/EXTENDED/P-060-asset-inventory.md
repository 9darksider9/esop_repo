# P-060 Asset Inventory

## Statement

All assets must be inventoried with defined ownership; unknown assets
are untrusted.

## Reasoning

Security controls cannot protect assets that are not known to exist.
Ownership ensures accountability for security posture, patching,
configuration, and incident response. Unowned assets drift without
maintenance and escape security governance.

Unknown assets are assumed hostile until verified. Inventory is the
foundation for all other asset-level controls.

## Justification

Breaches frequently originate from forgotten systems: shadow IT,
orphaned cloud resources, undocumented integrations, and inherited
infrastructure. These assets lack patching, monitoring, and access
review. Attackers specifically seek unmanaged assets because they
represent undefended entry points.

Without inventory, organizations cannot answer fundamental questions
about their attack surface.

## Operational Uses

- Automated asset discovery and reconciliation.
- Ownership assignment and verification.
- Integration with vulnerability and configuration management.
- Network access control based on inventory status.
- Incident response asset identification.

## Misuse / Abuse Risks

- Inventory becoming stale and losing operational value.
- Administrative burden of maintaining ownership records.
- Over-blocking legitimate assets due to inventory gaps.
- False confidence from incomplete discovery.

## Related Principles

- P-001 Telemetry Required
- P-061 Decommissioning Required
- P-062 Dependency Tracking

## Compliance Touchpoints

Placeholder
