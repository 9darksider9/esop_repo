# VIS-01.09 — Fail Open Collection

## Statement

Telemetry pipelines must fail open for collection and fail closed for
enforcement.

## Reasoning

Collection and enforcement have opposite failure mode requirements.
When collection fails, the priority is preserving data—buffering,
retrying, accepting degraded quality over loss. When enforcement fails,
the priority is safety—denying access until the control can be
restored.

Applying the wrong failure mode inverts security priorities: fail-closed
collection creates blind spots; fail-open enforcement creates bypasses.

## Justification

Telemetry pipelines under load must not drop events to maintain
throughput. Enforcement systems under load must not permit unauthorized
access to maintain availability. Confusion between these modes causes
either unacceptable data loss or unacceptable security bypass.

## Operational Uses

- Buffer sizing for collection burst capacity.
- Graceful degradation strategies for overloaded pipelines.
- Fail-closed defaults for authentication and authorization.
- Separate failure mode documentation for each system.
- Testing of failure behavior under load.

## Misuse / Abuse Risks

- Fail-open collection enabling denial-of-service through log flooding.
- Fail-closed enforcement causing availability incidents.
- Confusion when systems have mixed collection and enforcement roles.
- Difficulty tuning failure modes for edge cases.

## Related Principles

- VIS-01.07 Completeness Over Precision
- AUT-03.06 Automation Failure Safety
- RES-04.10 Silent Failure Unacceptable

## Compliance Touchpoints

Placeholder
