# VIS-01.12 — Unobservable Untrusted

## Statement

Systems that cannot be observed cannot be trusted.

## Reasoning

Trust requires verification. Verification requires observation.
Systems that resist observation—whether by design, configuration, or
failure—cannot demonstrate their security posture, cannot be validated
for correct operation, and cannot be investigated during incidents.

Unobservability is not a technical limitation to accept; it is a
security defect to remediate.

## Justification

Black-box systems create accountability gaps. Vendors that refuse
telemetry access, legacy systems without logging capability, and
encrypted channels without inspection all create zones where attackers
can operate without detection. Trust granted to unobservable systems
is faith, not security.

## Operational Uses

- Observability requirements in procurement and architecture review.
- Compensating controls for systems with limited observability.
- Risk acceptance documentation for unobservable systems.
- Network segmentation isolating unobservable zones.
- Roadmaps for improving observability of legacy systems.

## Misuse / Abuse Risks

- Rejecting necessary systems for observability limitations.
- Observability requirements exceeding privacy boundaries.
- Inspection capabilities creating new attack surfaces.
- Observability theater without actual analysis.

## Related Principles

- VIS-01.01 Telemetry Required
- VIS-01.02 Telemetry Implies Trust
- RES-04.01 Assume Compromise

## Compliance Touchpoints

Placeholder
