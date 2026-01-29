# AUT-03.02 — Intent and Execution Separation

## Statement

Humans approve intent; machines execute action.

## Reasoning

Human judgment is required for decisions involving context, risk
assessment, and policy interpretation. Human execution is unreliable
for tasks requiring speed, consistency, and scale. Security operations
must separate decision authority from execution mechanics.

Automated execution from approved intent reduces errors, increases speed,
and creates auditable consistency. Manual execution at scale guarantees
inconsistency and operator fatigue.

## Justification

Manual security operations cannot keep pace with modern attack velocity
or system complexity. Human operators introduce variance, make mistakes
under pressure, and cannot maintain consistent execution across thousands
of assets. Attackers exploit the gap between detection and response that
manual processes create.

Automation also provides auditability. Scripted actions produce
consistent logs; ad-hoc commands do not.

## Operational Uses

- Infrastructure as code for security configurations.
- Automated response playbooks triggered by detection.
- Policy-as-code enforcement pipelines.
- Self-healing systems that remediate known conditions.
- Approval workflows that gate automated execution.

## Misuse / Abuse Risks

- Automation amplifying errors at scale.
- Removing human oversight from high-consequence decisions.
- Brittle automation failing under novel conditions.
- Over-reliance on automation without understanding failure modes.

## Related Principles

- AUT-03.01 Eliminate Manual Execution
- AUT-03.04 Observable Automation
- AUT-03.05 AI Guardrails

## Compliance Touchpoints

Placeholder
