# Open Source Release Notes

This archive was prepared for public sharing as a legacy preservation project.

## What Was Sanitized

- Hard-coded service credentials were replaced with placeholder values.
- Customer or company hostnames were replaced with `example.com` style endpoints.
- IP addresses used for live integrations were replaced with documentation-only sample addresses from reserved ranges.
- Mailbox names, keyrings, user IDs, job card names, and owner identifiers were generalized.

## Placeholder Conventions

- `<SERVICE_USER>` and `<SERVICE_PASSWORD>` identify credentials that must come from a secure local source.
- `<ACCESS_KEY>` identifies an external API or partner key.
- `*.example.com` and `mail.example.net` are sample hostnames only.
- `192.0.2.x` addresses are documentation-only sample IP addresses.
- `<KEYRING_NAME>` and `<MAILBOX_NAME>` identify local CICS or security definitions that must be supplied by each installation.
- `SITE.*` and `USER0001` style names are generic stand-ins for local data set and user naming conventions.

## Remaining Site-Specific Areas To Review

- JCL data set names and high-level qualifiers.
- CICS APPLIDs, SYSIDs, terminal definitions, and auto-install tables.
- Printer, spool, SMTP, TCP/IP, VTAM, DB2, MQ, and CPSM resource names.
- Any business identifiers that may still be meaningful within your organization.

## Recommended Publication Process

1. Run a final manual review for ownership and licensing.
2. Confirm there is no production data, customer data, or private documentation mixed into the source.
3. Keep credentials and partner connection values out of the repository permanently.
4. If you later add build instructions, prefer symbolic JCL parameters and environment-specific sample members instead of real values.
