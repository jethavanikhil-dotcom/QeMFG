# AGENTS.md

## Cursor Cloud specific instructions

This is a static HTML/CSS CRM dashboard with no build system, no package manager, and no dependencies to install. The entire application consists of `index.html` and `styles.css`.

### Running the application

Serve the files with any static HTTP server from the workspace root:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/` in a browser.

### Key notes

- There are no automated tests, linting tools, or build steps configured in this repository.
- External assets (Google Fonts, Font Awesome) are loaded via CDN; the layout works without internet but icons and custom fonts will be missing.
- All charts are pure SVG/CSS (no JavaScript)—there is no interactive behavior beyond native HTML link/button highlighting.
