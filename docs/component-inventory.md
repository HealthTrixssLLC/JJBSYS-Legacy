# Component Inventory

This inventory is based on naming patterns and observed comments. Detailed descriptions should still be validated by mainframe and CICS experts.

## Prefix Groups

- `$GEN*`: build, generation, compile, or procedure-oriented JCL members
- `DFH*`: CICS samples, tables, exits, PLT members, and system-facing support
- `IEB*`: batch-to-CICS, EXCI bridge, and CICS resource access utilities
- `IEP*`: CICS operations and support utilities
- `IET*`: TCP/IP, SMTP, HTTP, UPS-style, and external integration utilities
- `IEW*`: CICS web interface support members
- `IEX*`: user exits
- `IEIAIT` / `IEMAIT`: terminal autoinstall support
- `OHCI*` / `OJCI*`: SMP/E, maintenance, or modification support artifacts
- `TCC*`: TCP/IP client/server examples or adjacent integration members

## Reviewer Note

Use this inventory as a map, not as a final authority. When in doubt, trace comments, COMMAREAs, transaction names, queue references, and related members.
