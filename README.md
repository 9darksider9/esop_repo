# Enterprise Security Operating Principles (ESOP)

## Foundations for Scalable Trust and Resilience

This repository defines the foundational principles governing how
security is designed, implemented, operated, measured, and evolved
across an enterprise environment.

Security is treated as a system of constraints, not a collection of
tools.

Principles guide architecture.\
Controls implement principles.\
Compliance validates controls.\
Telemetry validates reality.

---

## Principle Identifier Format

ESOP uses domain-scoped identifiers in the format:

```
<DOMAIN>-<DOMAIN_ID>.<PRINCIPLE_ID>
```

**Examples:**
- `VIS-01.01` — Telemetry Required
- `RES-04.05` — Recovery Exercised
- `ENG-05.11` — Secure Defaults

**Domain Prefixes:**
- `VIS-01` — Visibility, Telemetry, and Truth
- `IDN-02` — Identity, Authorization, and Trust
- `AUT-03` — Automation, Scale, and Human Limits
- `RES-04` — Resilience, Failure, and Blast Radius
- `ENG-05` — Engineering Discipline and Evidence
- `ETH-06` — Ethics, Data Stewardship, and Power

**Immutability Rule:** Once assigned, principle IDs are immutable. They
must never be reused, renumbered, or repurposed. See `docs/id-mapping.md`
for the complete mapping from legacy `P-###` identifiers.

---

## Purpose and Scope

ESOP establishes authoritative security principles for enterprise
operations. These principles are technology-agnostic, vendor-neutral,
and designed to remain stable across organizational changes.

**This is a living doctrine.** Principles evolve through governed
change processes as threats, technologies, and business contexts
change. Stability is valued; stagnation is not.

**Scope includes:**

- All systems, assets, and data under organizational control
- All personnel with access to organizational resources
- All third parties integrated into organizational operations
- All environments: production, development, and operational

**Scope excludes:**

- Implementation-specific controls (these derive from principles)
- Tool selection and vendor recommendations
- Compliance-specific audit procedures

## Principles to Controls to Compliance

Principles are abstract and durable. Controls are concrete and
contextual. Compliance validates that controls exist and function.

```
PRINCIPLE (Why)
    ↓
CONTROL (What)
    ↓
COMPLIANCE (Proof)
    ↓
TELEMETRY (Reality)
```

**Principles** define required security properties. They answer "what
must be true" without prescribing implementation.

**Controls** implement principles through specific mechanisms: policies,
configurations, procedures, or technical enforcement. A single principle
may require multiple controls. A single control may satisfy multiple
principles.

**Compliance** validates that controls are implemented and operating
effectively. Compliance evidence is derived from controls, not invented
independently.

**Telemetry** provides continuous validation that reality matches intent.
Compliance is periodic; telemetry is continuous.

## Operational Usage

### For Security Architecture

Use principles as decision criteria when evaluating designs. If a
proposed architecture violates a principle, the architecture must
change or a documented exception must be approved.

### For Engineering Teams

Reference principles when implementing security controls. Principles
define the required outcome; teams select appropriate mechanisms.
When in doubt, consult the owning security team.

### For Security Operations

Use principles to evaluate incidents and anomalies. Principle violations
indicate control failures. Control failures require remediation and
root cause analysis.

### For Compliance and Audit

Map audit requirements to principles first, then to implementing controls.
This ensures audit evidence reflects actual security posture rather than
checkbox compliance.

### For Leadership

Principles provide a stable vocabulary for security discussions.
Principle coverage metrics indicate architectural maturity. Principle
violation trends indicate operational risk.

## Repository Structure

```
/PRINCIPLES/
├── A-visibility/      Visibility, Telemetry, and Truth (VIS-01)
├── B-identity/        Identity, Authorization, and Trust (IDN-02)
├── C-automation/      Automation, Scale, and Human Limits (AUT-03)
├── D-resilience/      Resilience, Failure, and Blast Radius (RES-04)
├── E-engineering/     Engineering Discipline and Evidence (ENG-05)
└── F-ethics/          Ethics, Data Stewardship, and Power (ETH-06)

/COMPLIANCE/           Framework-specific validation scaffolding
/MAPPINGS/             Principle-to-control-framework mappings
/docs/                 Documentation including ID mapping
/GOVERNANCE.md         Change control and versioning policy
/ROADMAP.md            Planned expansion areas
```

---

## Principle Index

### VIS-01 — Visibility, Telemetry, and Truth

#### Canonical (VIS-01.01 to VIS-01.12)

- VIS-01.01 Telemetry Required
- VIS-01.02 Telemetry Implies Trust
- VIS-01.03 Telemetry Quality
- VIS-01.04 Forensic Retention
- VIS-01.05 Data Lineage
- VIS-01.06 Schema Drift Defect
- VIS-01.07 Completeness Over Precision
- VIS-01.08 Collection Gaps Alert
- VIS-01.09 Fail Open Collection
- VIS-01.10 Data Freshness
- VIS-01.11 Observable Decisions
- VIS-01.12 Unobservable Untrusted

#### Extended (VIS-01.13+)

- VIS-01.13 Audit Trail Mandatory
- VIS-01.14 Asset Inventory

### IDN-02 — Identity, Authorization, and Trust

#### Canonical (IDN-02.01 to IDN-02.12)

- IDN-02.01 Attributable Identity
- IDN-02.02 Anonymous Access Defect
- IDN-02.03 Machine Identity Risk
- IDN-02.04 Credential Hygiene
- IDN-02.05 Standing Privilege Debt
- IDN-02.06 Privilege Decay
- IDN-02.07 Explainable Authorization
- IDN-02.08 Identity Resilience
- IDN-02.09 Explicit Trust Boundaries
- IDN-02.10 Cross-Boundary Telemetry
- IDN-02.11 Continuous Validation
- IDN-02.12 Workload-Based Privilege

#### Extended (IDN-02.13+)

- IDN-02.13 Least Privilege
- IDN-02.14 Boundary Enforcement

### AUT-03 — Automation, Scale, and Human Limits

#### Canonical (AUT-03.01 to AUT-03.10)

- AUT-03.01 Eliminate Manual Execution
- AUT-03.02 Intent and Execution Separation
- AUT-03.03 Automate Repetition
- AUT-03.04 Observable Automation
- AUT-03.05 AI Guardrails
- AUT-03.06 Automation Failure Safety
- AUT-03.07 Human Toil Signal
- AUT-03.08 Complexity Compounds Risk
- AUT-03.09 Reliability Over Cleverness
- AUT-03.10 Understanding Over Action

### RES-04 — Resilience, Failure, and Blast Radius

#### Canonical (RES-04.01 to RES-04.10)

- RES-04.01 Assume Compromise
- RES-04.02 Blast Radius Measurable
- RES-04.03 Lateral Movement Visible
- RES-04.04 Shared Fate Justification
- RES-04.05 Recovery Exercised
- RES-04.06 Detection Over Prevention
- RES-04.07 Containment Automatable
- RES-04.08 Data Integrity Incidents
- RES-04.09 Recovery Objectives Validated
- RES-04.10 Silent Failure Unacceptable

#### Extended (RES-04.11+)

- RES-04.11 Proportionate Response
- RES-04.12 Rollback Capability
- RES-04.13 Vulnerabilities Are Contextual

### ENG-05 — Engineering Discipline and Evidence

#### Canonical (ENG-05.01 to ENG-05.10)

- ENG-05.01 Controls Declare Purpose
- ENG-05.02 Metrics Required
- ENG-05.03 Evidence Over Opinion
- ENG-05.04 Assumptions Tested
- ENG-05.05 Drift Detection
- ENG-05.06 Configuration Is Code
- ENG-05.07 Change Attribution
- ENG-05.08 Repeat Failures Systemic
- ENG-05.09 Security Debt Compounds
- ENG-05.10 Untestable Untrustworthy

#### Extended (ENG-05.11+)

- ENG-05.11 Secure Defaults
- ENG-05.12 Decommissioning Required
- ENG-05.13 Dependency Tracking
- ENG-05.14 Change Validation
- ENG-05.15 Baseline Enforcement
- ENG-05.16 Supply Chain Verification
- ENG-05.17 Baselines Are Required
- ENG-05.18 Drift Is a Security Signal
- ENG-05.19 Unmanaged Vulnerabilities Are Defects

### ETH-06 — Ethics, Data Stewardship, and Power

#### Canonical (ETH-06.01 to ETH-06.07)

- ETH-06.01 Data Collection Justified
- ETH-06.02 Data Access Auditable
- ETH-06.03 Data Minimization
- ETH-06.04 Transparency
- ETH-06.05 Power Asymmetry
- ETH-06.06 External Defensibility
- ETH-06.07 Non-Punitive Telemetry

#### Extended (ETH-06.08+)

- ETH-06.08 Vendor Assessment
