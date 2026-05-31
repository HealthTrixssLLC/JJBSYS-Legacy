# Review Guide

This repository should be reviewed as a historical CICS/mainframe archive, not as a production-ready software distribution.

## Suggested Review Approach

1. Start with [README.md](README.md).
2. Review [OPEN_SOURCE_RELEASE.md](OPEN_SOURCE_RELEASE.md).
3. Review the documentation site, especially the component inventory and modernization map.
4. Review source members by prefix to understand likely role and scope.
5. Look for any remaining site-specific values, operational assumptions, or unclear areas that need documentation.
6. Suggest documentation improvements through issues or pull requests.

## Prefix-Oriented Review Strategy

- Review `$GEN*` for build and generation JCL patterns.
- Review `DFH*` for CICS tables, exits, PLT members, and CICS support structures.
- Review `IEB*`, `IEP*`, and `IEX*` for batch integration, operational support, and exit behavior.
- Review `IET*` and `IEW*` for external integration, web support, and protocol handling patterns.
- Review `IEIAIT` and `IEMAIT` for terminal and autoinstall behavior.

## Public Review Safety

- Do not post secrets or sensitive findings publicly.
- If something appears operationally sensitive, report it privately using [SECURITY.md](SECURITY.md).
- Keep source conclusions cautious unless validated by CICS and z/OS experts.
