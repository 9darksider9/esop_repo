# P-035 Assume Compromise

## Statement

Compromise is assumed.

## Reasoning

No defense is absolute. Sophisticated attackers, supply chain
compromises, insider threats, and zero-day exploits will eventually
succeed. Security architecture must assume that some components are
already compromised and design for containment, detection, and recovery.

Assuming breach shifts focus from prevention alone to detection,
containment, and resilience. Systems designed only for prevention fail
catastrophically when prevention fails.

## Justification

Organizations that assume their perimeter is intact are consistently
surprised by breaches that have persisted for months or years. Flat
networks, implicit trust, and prevention-only controls allow attackers
to move freely once initial access is achieved.

Assume-compromise architectures limit blast radius, accelerate detection,
and enable recovery even when prevention fails.

## Operational Uses

- Network segmentation limiting lateral movement.
- Zero-trust access models requiring continuous verification.
- Detection controls focused on post-compromise behavior.
- Incident response planning and regular exercises.
- Encryption of data at rest assuming storage compromise.

## Misuse / Abuse Risks

- Fatalism that reduces investment in prevention.
- Overbuilding internal controls at the expense of usability.
- Paranoid architectures that impede legitimate operations.
- Assuming compromise without building detection capabilities.

## Related Principles

- P-036 Blast Radius Measurable
- P-037 Lateral Movement Visible
- P-039 Recovery Exercised

## Compliance Touchpoints

Placeholder
