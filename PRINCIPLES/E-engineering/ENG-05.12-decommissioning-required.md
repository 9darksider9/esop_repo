# ENG-05.12 — Decommissioning Required

## Statement

End-of-life assets must be securely decommissioned; abandoned assets are
liabilities.

## Reasoning

Systems accumulate entropy over time. Assets that are no longer actively
managed continue to expose credentials, network access, data, and attack
surface. Abandoned assets frequently retain privileged access, outdated
software, and undocumented dependencies.

Security requires not only secure creation and operation of assets, but
also secure retirement.

## Justification

A significant percentage of breaches originate from forgotten systems:
expired cloud resources, legacy virtual machines, unused SaaS tenants,
abandoned domains, orphaned storage buckets, or retired integrations that
retain credentials and connectivity. These assets escape monitoring,
patching, and ownership accountability.

Attackers actively search for abandoned infrastructure because it offers
low resistance and high persistence.

## Operational Uses

- Asset inventory lifecycle enforcement.
- Automated detection of inactive or orphaned resources.
- Credential revocation during decommissioning.
- Data sanitization and destruction verification.
- DNS, certificate, and account cleanup.

## Misuse / Abuse Risks

- Premature decommissioning causing production outages.
- Incomplete data destruction creating compliance exposure.
- Orphaned dependencies breaking downstream systems.
- Manual decommissioning errors without automation.

## Related Principles

- VIS-01.01 Telemetry Required
- VIS-01.14 Asset Inventory
- ENG-05.06 Configuration Is Code

## Compliance Touchpoints

Placeholder
