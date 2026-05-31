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
