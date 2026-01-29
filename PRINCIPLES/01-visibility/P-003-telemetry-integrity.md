# P-003 Telemetry Integrity

## Statement

Telemetry pipelines must be tamper-evident and independently verifiable.

## Reasoning

Telemetry that can be silently modified, deleted, or forged cannot be
trusted for security decisions, investigations, or compliance evidence.
Attackers with sufficient access will manipulate logs to cover their
tracks. Insiders with access to collection infrastructure can falsify
records.

Integrity requires cryptographic evidence that data has not been altered
since creation and that the chain of custody is verifiable.

## Justification

Post-compromise forensics frequently discover log tampering, timestamp
manipulation, or selective deletion. Systems that rely on
access-controlled storage without integrity verification cannot
distinguish between authentic records and attacker modifications.

Regulatory and legal proceedings require demonstrable chain of custody.
Telemetry without integrity controls may be inadmissible or unreliable.

## Operational Uses

- Cryptographic signing at the point of event generation.
- Append-only storage with immutability guarantees.
- Independent integrity verification separate from collection.
- Hash chaining or merkle structures for sequence verification.
- Separation of duties between producers and custodians.

## Misuse / Abuse Risks

- Performance overhead from cryptographic operations.
- Key management complexity introducing new failure modes.
- False confidence from integrity checks that only cover partial paths.
- Complexity preventing adoption in resource-constrained environments.

## Related Principles

- P-001 Telemetry Required
- P-002 No Missing Data
- P-022 Audit Trail Mandatory

## Compliance Touchpoints

Placeholder
