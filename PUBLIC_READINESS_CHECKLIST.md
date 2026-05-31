# Public Readiness Checklist

## Licensing

- [ ] Confirm the Apache 2.0 license is the intended public license.
- [ ] Confirm any third-party code or borrowed samples are compatible with public distribution.

## Ownership Review

- [ ] Confirm the repository can be publicly shared as a preservation archive.
- [ ] Confirm no restricted internal documentation is mixed into the source.

## Sensitive Value Review

- [ ] Review for remaining credentials, keys, private hostnames, user IDs, and operational identifiers.
- [ ] Review legacy comments for company-specific references or sensitive notes.
- [ ] Confirm no production data or customer information is present.

## Documentation Completeness

- [ ] README reflects archival and educational purpose.
- [ ] Disclaimer, contribution guide, and review guide are present.
- [ ] Component inventory and architecture notes are available.

## GitHub Pages

- [ ] `/docs` content is present and links correctly.
- [ ] GitHub Pages is enabled from `main` and `/docs`.

## Security Policy

- [ ] Security reporting instructions are documented.
- [ ] Public issue guidance warns against posting sensitive findings.

## Contribution Governance

- [ ] CODEOWNERS is present.
- [ ] Pull request template is present.
- [ ] Issue templates are present.
- [ ] Code of conduct is present.

## Branch Protection Recommendations

- [ ] Require pull requests before merging to `main`.
- [ ] Require code owner review where appropriate.
- [ ] Restrict direct pushes to `main`.
- [ ] Consider requiring status checks for documentation validation workflows if added later.

## Future Expert Review

- [ ] Request a CICS and z/OS expert pass for source classification.
- [ ] Request a final sanitization pass before broader promotion.
- [ ] Request modernization-oriented review notes for major component families.
