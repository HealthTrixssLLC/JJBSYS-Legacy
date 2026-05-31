# Architecture

This page gives a conceptual view of how the major legacy components relate. It is intended for review and orientation, not installation.

## Conceptual Flow

```text
Batch Jobs / JCL
      |
      v
EXCI Client and Bridge Programs
      |
      v
CICS Transactions / Server Programs
      |         |         |         |
      |         |         |         +-- CICS Web Interface / HTTP support
      |         |         +------------ TCP/IP and SMTP integration routines
      |         +---------------------- Files, queues, programs, and resources
      +-------------------------------- Operational tools, exits, and utilities
```

## Major Relationships

- Batch jobs and JCL appear to drive build, generation, and batch-triggered service patterns.
- EXCI bridge programs appear to let non-CICS or batch processes request controlled work from CICS.
- CICS programs appear to operate on queues, files, regions, and support transactions.
- Network-facing utilities extend the region into TCP/IP, SMTP, HTTP, and related external integration flows.
- Terminal support, exits, and PLT members reflect operational control and lifecycle behavior.
