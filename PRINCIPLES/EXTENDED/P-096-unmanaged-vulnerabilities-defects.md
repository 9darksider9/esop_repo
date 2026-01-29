# P-096 Unmanaged Vulnerabilities Are Defects

## Statement

Vulnerabilities without ownership, prioritization, or remediation strategy
are security defects.

## Reasoning

A vulnerability is not managed simply by being discovered. Vulnerabilities
require ownership to ensure accountability, prioritization to focus effort,
and remediation strategy to drive resolution. Vulnerabilities lacking any
of these elements exist in an unmanaged state where they neither get fixed
nor are explicitly accepted.

Unmanaged vulnerabilities accumulate until breach forces attention.

## Justification

Vulnerability backlogs grow when discovered issues lack clear owners or
remediation paths. Teams assume someone else will address them. Prioritization
disputes stall action. Without explicit strategy, vulnerabilities persist
indefinitely in a state of organizational neglect.

Every vulnerability must have an owner, a priority, and a path to resolution
or documented acceptance.

## Operational Uses

- Mandatory ownership assignment for all discovered vulnerabilities.
- Prioritization required within defined timeframe of discovery.
- Remediation strategy or risk acceptance documented for each finding.
- Unowned vulnerability metrics as security program health indicator.
- Escalation procedures for vulnerabilities lacking management.

## Misuse / Abuse Risks

- Administrative burden of managing low-risk vulnerabilities.
- Ownership assignment without corresponding remediation authority.
- Documentation theater substituting for actual remediation.
- Risk acceptance becoming default path to close findings.

## Related Principles

- P-095 Vulnerabilities Are Contextual
- P-053 Security Debt Compounds
- P-052 Repeat Failures Systemic

## Compliance Touchpoints

Placeholder
