# P-023 Continuous Validation

## Statement

Identity assertions must be continuously validated.

## Reasoning

Point-in-time authentication is insufficient. Session hijacking,
credential theft, and context changes can invalidate initial
authentication. Continuous validation ensures that identity assertions
remain valid throughout the access session, not just at its beginning.

Authentication is not a gate; it is a continuous requirement.

## Justification

Attackers steal session tokens, hijack authenticated connections, and
persist access beyond credential revocation. Authentication that
validates only at session start grants attackers unlimited time to
operate once initial access is obtained. Continuous validation limits
the window of exploitation.

## Operational Uses

- Session revalidation on sensitive operations.
- Context-aware authentication checking location, device, behavior.
- Token refresh with revalidation requirements.
- Real-time revocation checking.
- Behavioral anomaly triggering reauthentication.

## Misuse / Abuse Risks

- Friction from excessive revalidation prompts.
- Performance overhead from continuous checks.
- False positives from legitimate context changes.
- Revalidation bypasses for performance optimization.

## Related Principles

- P-013 Attributable Identity
- P-016 Credential Hygiene
- P-020 Identity Resilience

## Compliance Touchpoints

Placeholder
