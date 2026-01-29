# ENG-05.11 — Secure Defaults

## Statement

Default configurations must be secure without modification; insecure
defaults are defects.

## Reasoning

Most systems are deployed with default configurations. If defaults are
insecure, the majority of deployments will be insecure. Requiring
explicit hardening creates a gap between intended security and actual
security that scales with deployment volume.

Secure defaults shift the burden from operators to system designers.
Insecure defaults shift risk to every deployment.

## Justification

Large-scale vulnerability exploitation frequently targets default
configurations: default credentials, default ports, default permissions,
and default-enabled services. Attackers automate scanning for default
states because they represent predictable, widespread exposure.

Systems that require explicit hardening accumulate configuration debt
and create inconsistent security posture across deployments.

## Operational Uses

- Baseline hardening built into golden images.
- Default-deny network policies.
- Disabled-by-default for non-essential services.
- Strong default authentication requirements.
- Secure default permissions and access controls.

## Misuse / Abuse Risks

- Overly restrictive defaults breaking legitimate use cases.
- Documentation gaps for how to enable needed functionality.
- Drift from secure defaults during troubleshooting.
- False confidence that defaults alone provide complete protection.

## Related Principles

- IDN-02.13 Least Privilege
- ENG-05.06 Configuration Is Code
- ENG-05.15 Baseline Enforcement

## Compliance Touchpoints

Placeholder
