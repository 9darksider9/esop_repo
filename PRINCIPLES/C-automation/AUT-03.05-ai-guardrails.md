# AUT-03.05 — AI Guardrails

## Statement

AI systems must operate with deterministic guardrails.

## Reasoning

AI and machine learning systems introduce non-determinism and opacity
that traditional automation does not. When AI systems make or influence
security decisions, deterministic guardrails must constrain their
operation to prevent unbounded or inexplicable behavior.

AI amplifies capability; guardrails constrain risk.

## Justification

AI systems can produce unexpected outputs, learn incorrect patterns,
or be manipulated through adversarial inputs. Without guardrails, AI
systems may take actions that cannot be predicted, explained, or
reversed. Security-critical AI requires boundaries that limit damage
from AI failures or manipulation.

## Operational Uses

- Output validation for AI-driven decisions.
- Scope limits on AI-initiated actions.
- Human approval for high-consequence AI recommendations.
- Behavioral bounds that trigger alerts when exceeded.
- Explainability requirements for AI decision factors.

## Misuse / Abuse Risks

- Guardrails too restrictive to capture AI value.
- False confidence from guardrails that don't cover all failure modes.
- Gaming guardrails to bypass intended constraints.
- Guardrail maintenance falling behind model evolution.

## Related Principles

- AUT-03.04 Observable Automation
- AUT-03.06 Automation Failure Safety
- AUT-03.10 Understanding Over Action

## Compliance Touchpoints

Placeholder
