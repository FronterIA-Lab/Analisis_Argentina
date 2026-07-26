# Analisis_Argentina

## Cursor Cloud specific instructions

This repository is a **research document corpus**, not a software application. It contains
geopolitical / "soberanía cognitiva" research about Argentina (dossiers, PDFs, Markdown,
plain text) plus one self-contained static HTML dossier. There is intentionally:

- No package manager, dependencies, or lockfiles
- No build system, lint config, or automated tests
- No backend/frontend services or databases

Because of this, there is nothing to install (the update script is a no-op) and there are no
`build`/`test`/`lint` commands to run.

### Previewing the HTML dossier

The only runnable artifact is `DOSSIER_RACISMO_ARGENTINA.html` (fully self-contained, inline CSS).
Serve the repo root with Python's built-in static server (Python 3 is preinstalled — no deps needed):

```bash
python3 -m http.server 8080 --directory .
# then open http://localhost:8080/DOSSIER_RACISMO_ARGENTINA.html
```

Note: navigating to the bare directory listing (`http://localhost:8080/`) in Chrome can trigger
address-bar autocomplete that jumps straight to the dossier file; use the full file URL directly.

The other files (`.txt`, `.md`, `.pdf`) are source materials meant to be read/edited directly; no
server is required for them.
