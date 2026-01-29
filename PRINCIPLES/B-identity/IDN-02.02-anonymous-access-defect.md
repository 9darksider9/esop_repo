# IDN-02.02 — Anonymous Access Defect

## Statement

Anonymous access is a defect.

## Reasoning

Access without identity attribution creates accountability gaps.
Anonymous actors cannot be distinguished from attackers, cannot be
subject to access controls, cannot be monitored for anomalous behavior,
and cannot be held accountable for their actions.

Systems that permit anonymous access have chosen convenience over
security. This tradeoff must be explicit, documented, and minimized.

## Justification

Attackers exploit anonymous access to blend with legitimate traffic,
exfiltrate data without attribution, and establish persistence without
detection. Incident responders cannot scope compromises when they
cannot identify which actions were attacker-controlled.

## Operational Uses

- Authentication requirements for all system access.
- Audit logging of authentication bypass exceptions.
- Risk acceptance for any remaining anonymous access.
- Compensating controls for unavoidably anonymous contexts.
- Reduction roadmaps for legacy anonymous access.

## Misuse / Abuse Risks

- Authentication friction reducing legitimate usage.
- Authentication systems becoming single points of failure.
- Credential fatigue from excessive authentication requirements.
- Privacy concerns from universal identity tracking.

## Related Principles

- IDN-02.01 Attributable Identity
- IDN-02.10 Cross-Boundary Telemetry
- ETH-06.02 Data Access Auditable

## Compliance Touchpoints

Placeholder
