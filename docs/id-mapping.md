# ESOP ID Mapping (P-### → DOMAIN-##.##)

This document records the one-time migration from legacy `P-###` identifiers to the ESOP domain-scoped identifier format:

`<DOMAIN>-<DOMAIN_ID>.<PRINCIPLE_ID>`

Examples:
- `VIS-01.01`
- `RES-04.05`
- `ENG-05.11`

## Why the Change

The legacy global numbering scheme (`P-###`) does not scale as domains grow and evolve. Domain-scoped IDs preserve meaning at a glance, support extensibility, and avoid cross-domain numbering collisions.

## Immutability Rule

**Principle IDs are immutable.**
Once assigned, an ESOP principle ID must never be reused, renumbered, or repurposed. Deprecated principles retain their IDs.

## Domain Prefixes

- `VIS-01` — Visibility, Telemetry, and Truth
- `IDN-02` — Identity, Authorization, and Trust
- `AUT-03` — Automation, Scale, and Human Limits
- `RES-04` — Resilience, Failure, and Blast Radius
- `ENG-05` — Engineering Discipline and Evidence
- `ETH-06` — Ethics, Data Stewardship, and Power

## Complete Mapping Table

| Old ID | New ID | Domain | Status | Title | Path |
|--------|--------|--------|--------|-------|------|
| P-001 | VIS-01.01 | Visibility | Canonical | Telemetry Required | PRINCIPLES/A-visibility/VIS-01.01-telemetry-required.md |
| P-002 | VIS-01.02 | Visibility | Canonical | Telemetry Implies Trust | PRINCIPLES/A-visibility/VIS-01.02-telemetry-implies-trust.md |
| P-003 | VIS-01.03 | Visibility | Canonical | Telemetry Quality | PRINCIPLES/A-visibility/VIS-01.03-telemetry-quality.md |
| P-004 | VIS-01.04 | Visibility | Canonical | Forensic Retention | PRINCIPLES/A-visibility/VIS-01.04-forensic-retention.md |
| P-005 | VIS-01.05 | Visibility | Canonical | Data Lineage | PRINCIPLES/A-visibility/VIS-01.05-data-lineage.md |
| P-006 | VIS-01.06 | Visibility | Canonical | Schema Drift Defect | PRINCIPLES/A-visibility/VIS-01.06-schema-drift-defect.md |
| P-007 | VIS-01.07 | Visibility | Canonical | Completeness Over Precision | PRINCIPLES/A-visibility/VIS-01.07-completeness-over-precision.md |
| P-008 | VIS-01.08 | Visibility | Canonical | Collection Gaps Alert | PRINCIPLES/A-visibility/VIS-01.08-collection-gaps-alert.md |
| P-009 | VIS-01.09 | Visibility | Canonical | Fail Open Collection | PRINCIPLES/A-visibility/VIS-01.09-fail-open-collection.md |
| P-010 | VIS-01.10 | Visibility | Canonical | Data Freshness | PRINCIPLES/A-visibility/VIS-01.10-data-freshness.md |
| P-011 | VIS-01.11 | Visibility | Canonical | Observable Decisions | PRINCIPLES/A-visibility/VIS-01.11-observable-decisions.md |
| P-012 | VIS-01.12 | Visibility | Canonical | Unobservable Untrusted | PRINCIPLES/A-visibility/VIS-01.12-unobservable-untrusted.md |
| P-EXT-002 | VIS-01.13 | Visibility | Extended | Audit Trail Mandatory | PRINCIPLES/A-visibility/VIS-01.13-audit-trail-mandatory.md |
| P-060 (Ext) | VIS-01.14 | Visibility | Extended | Asset Inventory | PRINCIPLES/A-visibility/VIS-01.14-asset-inventory.md |
| P-013 | IDN-02.01 | Identity | Canonical | Attributable Identity | PRINCIPLES/B-identity/IDN-02.01-attributable-identity.md |
| P-014 | IDN-02.02 | Identity | Canonical | Anonymous Access Defect | PRINCIPLES/B-identity/IDN-02.02-anonymous-access-defect.md |
| P-015 | IDN-02.03 | Identity | Canonical | Machine Identity Risk | PRINCIPLES/B-identity/IDN-02.03-machine-identity-risk.md |
| P-016 | IDN-02.04 | Identity | Canonical | Credential Hygiene | PRINCIPLES/B-identity/IDN-02.04-credential-hygiene.md |
| P-017 | IDN-02.05 | Identity | Canonical | Standing Privilege Debt | PRINCIPLES/B-identity/IDN-02.05-standing-privilege-debt.md |
| P-018 | IDN-02.06 | Identity | Canonical | Privilege Decay | PRINCIPLES/B-identity/IDN-02.06-privilege-decay.md |
| P-019 | IDN-02.07 | Identity | Canonical | Explainable Authorization | PRINCIPLES/B-identity/IDN-02.07-explainable-authorization.md |
| P-020 | IDN-02.08 | Identity | Canonical | Identity Resilience | PRINCIPLES/B-identity/IDN-02.08-identity-resilience.md |
| P-021 | IDN-02.09 | Identity | Canonical | Explicit Trust Boundaries | PRINCIPLES/B-identity/IDN-02.09-explicit-trust-boundaries.md |
| P-022 | IDN-02.10 | Identity | Canonical | Cross-Boundary Telemetry | PRINCIPLES/B-identity/IDN-02.10-cross-boundary-telemetry.md |
| P-023 | IDN-02.11 | Identity | Canonical | Continuous Validation | PRINCIPLES/B-identity/IDN-02.11-continuous-validation.md |
| P-024 | IDN-02.12 | Identity | Canonical | Workload-Based Privilege | PRINCIPLES/B-identity/IDN-02.12-workload-based-privilege.md |
| P-EXT-001 | IDN-02.13 | Identity | Extended | Least Privilege | PRINCIPLES/B-identity/IDN-02.13-least-privilege.md |
| P-092 | IDN-02.14 | Identity | Extended | Boundary Enforcement | PRINCIPLES/B-identity/IDN-02.14-boundary-enforcement.md |
| P-025 | AUT-03.01 | Automation | Canonical | Eliminate Manual Execution | PRINCIPLES/C-automation/AUT-03.01-eliminate-manual-execution.md |
| P-026 | AUT-03.02 | Automation | Canonical | Intent and Execution Separation | PRINCIPLES/C-automation/AUT-03.02-intent-execution-separation.md |
| P-027 | AUT-03.03 | Automation | Canonical | Automate Repetition | PRINCIPLES/C-automation/AUT-03.03-automate-repetition.md |
| P-028 | AUT-03.04 | Automation | Canonical | Observable Automation | PRINCIPLES/C-automation/AUT-03.04-observable-automation.md |
| P-029 | AUT-03.05 | Automation | Canonical | AI Guardrails | PRINCIPLES/C-automation/AUT-03.05-ai-guardrails.md |
| P-030 | AUT-03.06 | Automation | Canonical | Automation Failure Safety | PRINCIPLES/C-automation/AUT-03.06-automation-failure-safety.md |
| P-031 | AUT-03.07 | Automation | Canonical | Human Toil Signal | PRINCIPLES/C-automation/AUT-03.07-human-toil-signal.md |
| P-032 | AUT-03.08 | Automation | Canonical | Complexity Compounds Risk | PRINCIPLES/C-automation/AUT-03.08-complexity-compounds-risk.md |
| P-033 | AUT-03.09 | Automation | Canonical | Reliability Over Cleverness | PRINCIPLES/C-automation/AUT-03.09-reliability-over-cleverness.md |
| P-034 | AUT-03.10 | Automation | Canonical | Understanding Over Action | PRINCIPLES/C-automation/AUT-03.10-understanding-over-action.md |
| P-035 | RES-04.01 | Resilience | Canonical | Assume Compromise | PRINCIPLES/D-resilience/RES-04.01-assume-compromise.md |
| P-036 | RES-04.02 | Resilience | Canonical | Blast Radius Measurable | PRINCIPLES/D-resilience/RES-04.02-blast-radius-measurable.md |
| P-037 | RES-04.03 | Resilience | Canonical | Lateral Movement Visible | PRINCIPLES/D-resilience/RES-04.03-lateral-movement-visible.md |
| P-038 | RES-04.04 | Resilience | Canonical | Shared Fate Justification | PRINCIPLES/D-resilience/RES-04.04-shared-fate-justification.md |
| P-039 | RES-04.05 | Resilience | Canonical | Recovery Exercised | PRINCIPLES/D-resilience/RES-04.05-recovery-exercised.md |
| P-040 | RES-04.06 | Resilience | Canonical | Detection Over Prevention | PRINCIPLES/D-resilience/RES-04.06-detection-over-prevention.md |
| P-041 | RES-04.07 | Resilience | Canonical | Containment Automatable | PRINCIPLES/D-resilience/RES-04.07-containment-automatable.md |
| P-042 | RES-04.08 | Resilience | Canonical | Data Integrity Incidents | PRINCIPLES/D-resilience/RES-04.08-data-integrity-incidents.md |
| P-043 | RES-04.09 | Resilience | Canonical | Recovery Objectives Validated | PRINCIPLES/D-resilience/RES-04.09-recovery-objectives-validated.md |
| P-044 | RES-04.10 | Resilience | Canonical | Silent Failure Unacceptable | PRINCIPLES/D-resilience/RES-04.10-silent-failure-unacceptable.md |
| P-EXT-004 | RES-04.11 | Resilience | Extended | Proportionate Response | PRINCIPLES/D-resilience/RES-04.11-proportionate-response.md |
| P-071 | RES-04.12 | Resilience | Extended | Rollback Capability | PRINCIPLES/D-resilience/RES-04.12-rollback-capability.md |
| P-095 | RES-04.13 | Resilience | Extended | Vulnerabilities Are Contextual | PRINCIPLES/D-resilience/RES-04.13-vulnerabilities-contextual.md |
| P-045 | ENG-05.01 | Engineering | Canonical | Controls Declare Purpose | PRINCIPLES/E-engineering/ENG-05.01-controls-declare-purpose.md |
| P-046 | ENG-05.02 | Engineering | Canonical | Metrics Required | PRINCIPLES/E-engineering/ENG-05.02-metrics-required.md |
| P-047 | ENG-05.03 | Engineering | Canonical | Evidence Over Opinion | PRINCIPLES/E-engineering/ENG-05.03-evidence-over-opinion.md |
| P-048 | ENG-05.04 | Engineering | Canonical | Assumptions Tested | PRINCIPLES/E-engineering/ENG-05.04-assumptions-tested.md |
| P-049 | ENG-05.05 | Engineering | Canonical | Drift Detection | PRINCIPLES/E-engineering/ENG-05.05-drift-detection.md |
| P-050 | ENG-05.06 | Engineering | Canonical | Configuration Is Code | PRINCIPLES/E-engineering/ENG-05.06-configuration-is-code.md |
| P-051 | ENG-05.07 | Engineering | Canonical | Change Attribution | PRINCIPLES/E-engineering/ENG-05.07-change-attribution.md |
| P-052 | ENG-05.08 | Engineering | Canonical | Repeat Failures Systemic | PRINCIPLES/E-engineering/ENG-05.08-repeat-failures-systemic.md |
| P-053 | ENG-05.09 | Engineering | Canonical | Security Debt Compounds | PRINCIPLES/E-engineering/ENG-05.09-security-debt-compounds.md |
| P-054 | ENG-05.10 | Engineering | Canonical | Untestable Untrustworthy | PRINCIPLES/E-engineering/ENG-05.10-untestable-untrustworthy.md |
| P-EXT-003 | ENG-05.11 | Engineering | Extended | Secure Defaults | PRINCIPLES/E-engineering/ENG-05.11-secure-defaults.md |
| P-061 (Ext) | ENG-05.12 | Engineering | Extended | Decommissioning Required | PRINCIPLES/E-engineering/ENG-05.12-decommissioning-required.md |
| P-062 | ENG-05.13 | Engineering | Extended | Dependency Tracking | PRINCIPLES/E-engineering/ENG-05.13-dependency-tracking.md |
| P-072 | ENG-05.14 | Engineering | Extended | Change Validation | PRINCIPLES/E-engineering/ENG-05.14-change-validation.md |
| P-082 | ENG-05.15 | Engineering | Extended | Baseline Enforcement | PRINCIPLES/E-engineering/ENG-05.15-baseline-enforcement.md |
| P-091 | ENG-05.16 | Engineering | Extended | Supply Chain Verification | PRINCIPLES/E-engineering/ENG-05.16-supply-chain-verification.md |
| P-093 | ENG-05.17 | Engineering | Extended | Baselines Are Required | PRINCIPLES/E-engineering/ENG-05.17-baselines-required.md |
| P-094 | ENG-05.18 | Engineering | Extended | Drift Is a Security Signal | PRINCIPLES/E-engineering/ENG-05.18-drift-security-signal.md |
| P-096 | ENG-05.19 | Engineering | Extended | Unmanaged Vulnerabilities Are Defects | PRINCIPLES/E-engineering/ENG-05.19-unmanaged-vulnerabilities-defects.md |
| P-055 | ETH-06.01 | Ethics | Canonical | Data Collection Justified | PRINCIPLES/F-ethics/ETH-06.01-data-collection-justified.md |
| P-056 | ETH-06.02 | Ethics | Canonical | Data Access Auditable | PRINCIPLES/F-ethics/ETH-06.02-data-access-auditable.md |
| P-057 | ETH-06.03 | Ethics | Canonical | Data Minimization | PRINCIPLES/F-ethics/ETH-06.03-data-minimization.md |
| P-058 | ETH-06.04 | Ethics | Canonical | Transparency | PRINCIPLES/F-ethics/ETH-06.04-transparency.md |
| P-059 | ETH-06.05 | Ethics | Canonical | Power Asymmetry | PRINCIPLES/F-ethics/ETH-06.05-power-asymmetry.md |
| P-060 | ETH-06.06 | Ethics | Canonical | External Defensibility | PRINCIPLES/F-ethics/ETH-06.06-external-defensibility.md |
| P-061 | ETH-06.07 | Ethics | Canonical | Non-Punitive Telemetry | PRINCIPLES/F-ethics/ETH-06.07-non-punitive-telemetry.md |
| P-090 | ETH-06.08 | Ethics | Extended | Vendor Assessment | PRINCIPLES/F-ethics/ETH-06.08-vendor-assessment.md |

> **Status** is either `Canonical` or `Extended`.
