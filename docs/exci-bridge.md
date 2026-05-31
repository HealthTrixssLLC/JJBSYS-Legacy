# EXCI Bridge

EXCI is a bridge pattern that lets a batch or non-CICS process ask CICS to perform work on its behalf.

## Conceptual Flow

```text
Batch Job
  ->
EXCI Client
  ->
CICS Transaction / Server Program
  ->
CICS File / Queue / Program
  ->
Response
```

## Why It Matters

- It centralizes CICS-side handling.
- It reduces the need for direct external manipulation of internal CICS resources.
- It is a useful historical pattern for understanding controlled transaction access before modern API layers.

## Business Problem It Solved

Organizations often need overnight jobs, scheduled processes, reporting systems, and adjacent applications to use the same trusted business logic that powers online transaction systems. Without a bridge model, that can lead to duplicate logic, inconsistent outcomes, and higher operational risk.

This pattern helps solve that by letting batch and external workloads call into the same controlled CICS execution path.

## Why This Was Innovative And Successful

- It preserved the value of the core system instead of forcing duplication outside it.
- It gave the organization a way to expand usage of CICS services without opening uncontrolled access paths.
- It supported scale by allowing many business processes to reuse a stable transaction layer.

## Strengths

- Consistency: the same business rules can be reused across different channels.
- Control: access is mediated through known service points.
- Auditability: operational teams can reason about where business work is executed.
- Longevity: it is an early example of the same design instinct later seen in service gateways and APIs.
