# VIS-01.01 — Telemetry Required

## Statement

Every asset must produce authenticated telemetry or be removed from the
environment.

## Reasoning

Security depends on the ability to observe, attribute, and reconstruct
system behavior. Assets that do not emit trustworthy telemetry cannot be
monitored for compromise, cannot be validated for correct operation, and
cannot be investigated after failure or incident. Unobservable systems
introduce asymmetric risk where attackers operate without detection while
defenders operate without evidence.

Authenticated telemetry ensures that events are attributable,
tamper-resistant, and temporally consistent. Without these properties,
data cannot be trusted to drive automated controls, investigations, or
compliance evidence.

## Justification

Most material security failures exploit blind spots: unmanaged devices,
shadow SaaS, undocumented integrations, legacy appliances, orphaned
service accounts, or misconfigured collectors. In many incidents, the
inability to reconstruct timelines or validate system behavior materially
increases blast radius, recovery time, regulatory exposure, and
operational cost.

Attackers deliberately target logging infrastructure, disable telemetry,
or exploit unmonitored assets to maintain persistence. Treating telemetry
as optional guarantees undetected failure modes.

## Operational Uses

- Asset onboarding gates telemetry validation prior to production approval.
- CI/CD pipelines enforce logging contracts for all deployed services.
- Network segmentation isolates assets that cannot meet telemetry
  requirements.
- Procurement standards require verifiable telemetry capabilities.
- Incident response prioritizes restoration of telemetry pipelines.

## Misuse / Abuse Risks

- Excessive data collection without data minimization or retention
  governance.
- False confidence if telemetry integrity is not cryptographically
  protected.
- Cost explosion if collection is not aligned to operational value.
- Noise overload if schema discipline and filtering are weak.

## Related Principles

- VIS-01.02 Telemetry Implies Trust
- VIS-01.07 Completeness Over Precision
- VIS-01.12 Unobservable Untrusted

## Compliance Touchpoints

Placeholder
