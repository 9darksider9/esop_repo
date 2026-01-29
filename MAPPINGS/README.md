# Mappings

This directory contains mappings from ESOP principles to control
frameworks and compliance requirements.

## Purpose

Mappings establish traceability between abstract principles and concrete
implementations. They answer:

- Which controls implement which principles?
- Which compliance requirements are satisfied by which controls?
- What evidence demonstrates principle adherence?

## Principle → Control → Compliance Flow

```
PRINCIPLE (Why)
    ↓
CONTROL (What)
    ↓
COMPLIANCE (Proof)
```

**Principles** define required security properties. They are stable and
technology-agnostic.

**Controls** implement principles through specific mechanisms. A single
principle may require multiple controls. A single control may satisfy
multiple principles.

**Compliance** validates that controls exist and operate effectively.
Compliance evidence derives from control operation, not from principles
directly.

## Mapping Evolution

Mappings evolve separately from principles:

- Principles change rarely and require governance review.
- Control mappings change as implementations evolve.
- Compliance mappings change as regulatory requirements change.

A principle change may invalidate existing mappings. Mapping changes do
not affect principles.

## Status

Mappings are not yet populated. This directory contains scaffolding for
future mapping work.

When mappings are added, they will follow this structure:

```
/MAPPINGS/
├── README.md           (this file)
├── controls/           (principle-to-control mappings)
└── frameworks/         (control-to-framework mappings)
```
