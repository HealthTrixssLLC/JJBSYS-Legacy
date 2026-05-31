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
- `architecture.md`: Markdown architecture overview
- `architecture.html`: high-level conceptual architecture
- `component-inventory.md`: Markdown component inventory
- `component-inventory.html`: component grouping by naming pattern
- `exci-bridge.md`: Markdown EXCI bridge explanation
- `exci-bridge.html`: EXCI bridge explanation
- `cics-operations.md`: Markdown operations overview
- `cics-operations.html`: CICS operations overview
- `tcpip-smtp-web.md`: Markdown network, SMTP, and web overview
- `tcpip-smtp-web.html`: network, SMTP, and web integration overview
- `modernization-map.md`: Markdown modernization direction map
- `modernization-map.html`: modernization direction map
- `author-legacy.md`: Markdown legacy and attribution page
- `author-legacy.html`: legacy and attribution page
- `styles.css`: shared site styling

## Enable GitHub Pages

In repository settings:

1. Open `Settings`.
2. Open `Pages`.
3. Under `Build and deployment`, choose `Deploy from branch`.
4. Select branch `main`.
5. Select folder `/docs`.
6. Save the configuration.
