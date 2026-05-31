# Architecture

This page gives a conceptual view of how the major legacy components relate. It is intended for review and orientation, not installation.

## Business View

At a business level, this architecture appears designed to keep high-volume operational work reliable, centralized, and governable. Instead of letting every process interact with core data in its own way, it channels work through controlled CICS services and operational utilities.

That matters because it helps organizations:

- Reduce operational risk by standardizing how critical work is performed.
- Reuse proven transaction logic across batch, online, and integration channels.
- Support growth without rebuilding the core business system for every new interface.
- Keep mission-critical processing visible to operations teams instead of scattering it across disconnected tools.

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

## Problems This Helped Solve

- Integrating older core systems with new business workflows without rewriting everything.
- Protecting core business logic by routing access through managed service points.
- Supporting both scheduled and real-time work in the same operating environment.
- Giving operations teams a repeatable, supportable control model for essential business processing.

## Why This Was Effective

- It separates access patterns from core business execution.
- It favors controlled integration over ad hoc direct access.
- It reflects an engineering style built around reliability, observability, and long-term maintainability.
