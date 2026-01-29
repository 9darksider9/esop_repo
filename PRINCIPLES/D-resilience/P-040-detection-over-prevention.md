# P-040 Detection Over Prevention

## Statement

Time-to-detect matters more than time-to-prevent.

## Reasoning

Prevention will eventually fail. When it does, the duration of
undetected compromise determines the damage. Reducing detection time
limits attacker dwell time, constrains blast radius, and enables
faster recovery. Investing only in prevention without detection
guarantees extended compromise.

Prevention is valuable; detection is essential.

## Justification

Industry data consistently shows that breaches are detected months
after initial compromise. During this dwell time, attackers establish
persistence, exfiltrate data, and expand access. Organizations that
prioritize detection reduce dwell time and limit damage even when
prevention fails.

## Operational Uses

- Detection coverage metrics as primary security indicators.
- Mean time to detect as key performance metric.
- Investment prioritization toward detection capabilities.
- Detection-focused architecture reviews.
- Assume-breach detection scenarios in threat modeling.

## Misuse / Abuse Risks

- Underinvesting in prevention because detection exists.
- Detection fatigue from high false positive rates.
- Detection metrics gamed without improving actual detection.
- Detection investment without response capability investment.

## Related Principles

- P-035 Assume Compromise
- P-041 Containment Automatable
- P-044 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
