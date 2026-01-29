# Governance

All principles are version controlled. Changes require peer review and
documented justification. Deprecated principles remain archived.
Emergency changes require post-hoc review.

---

## Change Proposal Workflow

### 1. Proposal

Changes to principles require a written proposal containing:

- **Principle ID** (existing) or **proposed ID** (new)
- **Current statement** (if modifying existing)
- **Proposed statement**
- **Justification** explaining why the change is necessary
- **Impact assessment** identifying affected controls and systems

Proposals are submitted as pull requests to this repository.

### 2. Review

All proposals require review by:

- At least one security architect
- At least one operational stakeholder
- The principle domain owner (if established)

Reviewers evaluate:

- Alignment with existing principles (no contradiction)
- Clarity and enforceability of language
- Operational feasibility
- Absence of tool/vendor specificity

### 3. Approval

Approval requires:

- All required reviewers have approved
- No unresolved objections
- Justification is documented in the commit history

### 4. Implementation

Approved changes are merged to the main branch. Downstream control
owners are notified of changes affecting their domains.

## Review Expectations

Reviewers must respond within **5 business days** of assignment.

Reviews must address:

- **Accuracy**: Does the principle correctly describe the requirement?
- **Atomicity**: Does the principle contain exactly one idea?
- **Enforceability**: Can compliance with this principle be verified?
- **Overlap**: Does this duplicate or contradict existing principles?
- **Scope**: Is this principle appropriately scoped (not too broad or narrow)?

Reviewers may approve, request changes, or reject with documented reasoning.

## Versioning Approach

Principles are versioned through Git history. The repository does not
use semantic versioning for individual principles.

**Version tracking:**

- Each principle file's Git history constitutes its version history
- Significant changes should include descriptive commit messages
- The repository may be tagged for milestone releases

**Principle numbering:**

- Principle IDs (P-XXX) are permanent and never reused
- Gaps in numbering are intentional and reserved for future use
- Renumbering existing principles is prohibited

## Deprecation Policy

Principles are deprecated rather than deleted when they become obsolete.

**Deprecation process:**

1. Proposal submitted with justification for deprecation
2. Standard review process applies
3. If approved, principle file is moved to `/PRINCIPLES/_deprecated/`
4. Deprecated principles retain their ID permanently
5. A deprecation notice is added to the principle file

**Deprecation notice format:**

```
> **DEPRECATED:** [Date] - [Reason]
> Superseded by: [Principle ID] (if applicable)
```

Deprecated principles remain readable for historical reference and audit
continuity.

## Emergency Change Handling

Emergency changes are permitted when a principle:

- Contains a demonstrable error creating immediate risk
- Conflicts with legal or regulatory requirements with imminent deadlines
- Enables active exploitation

**Emergency process:**

1. Change is implemented by authorized personnel
2. Change is documented with emergency justification
3. Post-hoc review is conducted within **48 hours**
4. Standard review is completed within **5 business days**

Emergency changes that fail post-hoc review are reverted.

**Authorization:** Emergency changes require approval from the security
executive or designated delegate. The authorizing party is documented
in the commit.

## Exceptions

Individual systems or teams may request exceptions to specific principles.

**Exception requirements:**

- Written justification documenting why compliance is not feasible
- Risk assessment identifying exposure created by the exception
- Compensating controls mitigating identified risks
- Expiration date requiring renewal or remediation
- Approval from principle domain owner and security leadership

Exceptions are tracked outside this repository in the organization's
risk register.
