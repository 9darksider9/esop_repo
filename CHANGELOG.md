# Changelog

All notable changes to the Enterprise Security Operating Principles
repository are documented in this file.

## v3.0.0

- Migrated all principle IDs from P-### to domain-scoped format
- New ID scheme: `<DOMAIN>-<DOMAIN_ID>.<PRINCIPLE_ID>`
- Domain prefixes:
  - VIS-01: Visibility, Telemetry, and Truth
  - IDN-02: Identity, Authorization, and Trust
  - AUT-03: Automation, Scale, and Human Limits
  - RES-04: Resilience, Failure, and Blast Radius
  - ENG-05: Engineering Discipline and Evidence
  - ETH-06: Ethics, Data Stewardship, and Power
- Moved EXTENDED principles into domain folders
- Removed separate EXTENDED directory
- Created docs/id-mapping.md with complete legacy ID mapping
- Principle IDs are now immutable

## v2.0.0

- Expanded to 61 canonical principles aligned to authoritative list
- Reorganized into six thematic sections:
  - A: Visibility, Telemetry, and Truth (VIS-01.01 to VIS-01.12)
  - B: Identity, Authorization, and Trust (IDN-02.01 to IDN-02.12)
  - C: Automation, Scale, and Human Limits (AUT-03.01 to AUT-03.10)
  - D: Resilience, Failure, and Blast Radius (RES-04.01 to RES-04.10)
  - E: Engineering Discipline and Evidence (ENG-05.01 to ENG-05.10)
  - F: Ethics, Data Stewardship, and Power (ETH-06.01 to ETH-06.07)
- Created EXTENDED principles for non-canonical supplementary principles
- Updated README with complete principle index
- All principles follow consistent template structure

## v1.0.0

- Initial ESOP release
- 30 foundational principles across 10 domains
- Governance framework established
- Compliance scaffolding created (NIST 800-53, ISO 27001, SOC2, HIPAA,
  PCI-DSS)
- Repository structure formalized
