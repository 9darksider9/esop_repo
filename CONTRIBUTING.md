# Contributing to ESOP

This document describes how to propose changes to the Enterprise Security
Operating Principles repository.

## How to Propose a Principle Change

1. **Open an issue** describing the proposed change and its justification.
2. **Fork the repository** and create a branch for your change.
3. **Submit a pull request** with:
   - The modified principle file(s)
   - A clear description of what changed and why
   - Impact assessment identifying affected controls or systems
4. **Address review feedback** from required reviewers.

All changes require peer review per GOVERNANCE.md.

## What Qualifies as a Principle vs a Control

**Principles** are abstract, durable, and technology-agnostic. They define
what must be true without prescribing implementation.

- "Every action must have an attributable identity" is a principle.
- "Use SAML 2.0 for SSO" is a control.

**Controls** are concrete, contextual, and implementation-specific. They
describe how to achieve a principle.

If your proposal specifies a tool, vendor, protocol, or implementation
mechanism, it belongs in control documentation, not in ESOP.

## Review Expectations

All principle changes require review by:

- At least one security architect
- At least one operational stakeholder
- The principle domain owner (if established)

Reviewers evaluate alignment, clarity, enforceability, and overlap.
See GOVERNANCE.md for detailed review criteria.

Reviews must be completed within 5 business days.

## Versioning Expectations

- Principle IDs (P-XXX) are permanent and never reused.
- The repository uses Git history for version tracking.
- Significant releases may be tagged (e.g., v1.0.0, v1.1.0).
- Individual principles are not separately versioned.

Deprecated principles are moved to `/PRINCIPLES/_deprecated/` and retain
their IDs permanently.
