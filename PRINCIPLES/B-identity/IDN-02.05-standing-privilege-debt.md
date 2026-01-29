# IDN-02.05 — Standing Privilege Debt

## Statement

Standing privilege is a security debt.

## Reasoning

Privileges that exist continuously—whether or not they are being
used—represent accumulated risk. Standing privilege enables
instantaneous exploitation upon credential compromise. Each standing
privilege is a loan against future security that accrues interest
over time.

Just-in-time privilege reduces the attack surface by eliminating
standing access that is not actively required.

## Justification

Attackers seek accounts with standing privileges because they provide
immediate capability upon compromise. Privilege that must be requested
and granted creates friction that slows attackers and generates
detectable signals. Organizations with extensive standing privilege
carry material security debt.

## Operational Uses

- Just-in-time access elevation workflows.
- Standing privilege inventory and reduction programs.
- Privilege age tracking and decay enforcement.
- Exception documentation for necessary standing privileges.
- Metrics on standing versus just-in-time access.

## Misuse / Abuse Risks

- JIT overhead slowing legitimate operations.
- Approval bottlenecks during incidents.
- Standing privilege exceptions accumulating.
- Shadow access bypassing JIT controls.

## Related Principles

- IDN-02.06 Privilege Decay
- IDN-02.04 Credential Hygiene
- IDN-02.12 Workload-Based Privilege

## Compliance Touchpoints

Placeholder
