# AGENTS.md

## Cursor Cloud specific instructions

### Project overview
This is **LegalBD**, a single-page static marketing website for a Bangladeshi legal services firm. The entire site is a single `index.html` file (~97 KB) with inline CSS and JavaScript — no build system, no package manager, no backend, no database.

### Running the dev server
Serve the site with any static HTTP server, e.g.:
```
python3 -m http.server 8080
```
Then open `http://localhost:8080/` in Chrome. No dependencies to install.

### Lint / Test / Build
- **Lint**: No linter configured. You can optionally validate HTML with an external tool, but none is part of the project.
- **Tests**: No automated test framework. Manual browser testing is the only verification method.
- **Build**: No build step — the site is served as-is.

### Notes
- The contact form submission is simulated client-side with `setTimeout`; there is no backend endpoint.
- External CDN dependency: Google Fonts (`Hind Siliguri`, `Inter`). The site degrades gracefully without internet (falls back to system fonts).
- The site is intended for deployment on GitHub Pages.
