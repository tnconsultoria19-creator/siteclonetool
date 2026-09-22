# WebCraft Studio

WebCraft Studio is the fixed-template website package compiler.

## Workflow

1. ChatGPT receives the raw business information.
2. ChatGPT produces one complete **Website Package JSON** using Schema 5.0.
3. This app accepts that package directly.
4. The locked prototype is populated without rebuilding its layout.
5. The app provides a live preview and exports a standalone `index.html`.
6. The ZIP export is packaged as `projectdomain/index.html`.

Gemini is not part of this workflow.

## Source of truth

The visual prototype remains locked. Content changes are driven by the Website Package JSON.

## Repository

- `app/website-generator.html` — production generator UI and compiler.
- `templates/original-template.html` — exact extracted prototype source currently embedded by the compiler.
- `schemas/website-schema.json` — canonical Schema 5.0 structure.
- `samples/sample-business.json` — test package.
- `reference/preview.html` — reference preview artifact.
- `docs/Webcraft CRM System.txt` — existing CRM specification.
- `index.html` — GitHub Pages entry point.

No Node, React, Vite or build step is required for the generator itself.
