# Docs Site

The `docs/` directory contains the static GitHub Pages site for the repository.

## Best Way To Read The Docs

- For the rendered site experience, use GitHub Pages:
  [https://healthtrixssllc.github.io/JJBSYS-Legacy/](https://healthtrixssllc.github.io/JJBSYS-Legacy/)
- For browsing inside the GitHub repository itself, start with [index.md](index.md).

GitHub repository views do not reliably render standalone `.html` files as pages, so the repository includes Markdown companion documents for the key sections.

## Structure

- `index.md`: Markdown landing page for GitHub repo browsing
- `index.html`: project overview and navigation hub
- `review/`: architecture and high-level review guides
- `integration/`: EXCI, TCP/IP, SMTP, web, and external integration docs
- `operations/`: CICS operations and region-support docs
- `strategy/`: modernization and forward-looking documentation
- `legacy/`: author and preservation context
- `reference/`: component inventory and reviewer manifest
- `reference/review-manifest.md`: reviewer map for finding relevant docs and source families
- `reference/review-manifest.json`: machine-readable version of the reviewer map
- `styles.css`: shared site styling

## Enable GitHub Pages

In repository settings:

1. Open `Settings`.
2. Open `Pages`.
3. Under `Build and deployment`, choose `Deploy from branch`.
4. Select branch `main`.
5. Select folder `/docs`.
6. Save the configuration.
