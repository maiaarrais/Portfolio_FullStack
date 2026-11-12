# Maia Arrais — Engineering Portfolio

A responsive engineering portfolio for Maia's application to **BETA Technologies — Software Engineer, Customer Products, Digital Ops**. The visual design follows the updated resume: white surfaces, muted teal, slate typography, generous spacing, and fine dividers.

## What a reviewer can explore

- **Flow Studio:** Flask APIs, JavaScript Fetch requests, validation, capacity checks, and JSON persistence.
- **Rising Intentions:** a MongoDB-backed submission and statistics API connected to a shared visualization.
- **Ollama Classroom:** a real Unity demo of local LLM dialogue, bounded conversation context, and HTTP integration.
- **Long-Distance Bracelet:** dedicated documentation with original photos, engineering notes, and an interactive device-communication walkthrough.
- Additional work: 3D LED Box, Learning Experience Platform, and You As I Made.

Each featured project opens an accessible native dialog with original media, problem framing, personal contribution, implementation details, an architecture summary, tradeoffs, limitations, and next steps. Project source links lead to the existing repositories. Resume download and email contact work without a backend.

## Run locally

Requires Node.js 20.19+ or 22.12+.

```sh
npm ci
npm run dev -- --host 0.0.0.0 --port 4173
```

## Build

```sh
npm run build
npm run preview
```

Static output is in `dist/client/`. The bundled build also retains optional Sites-compatible output; no Sites publication is required.

For this repository's GitHub Pages path:

```sh
GITHUB_PAGES=true npm run build
```

This sets the base path to `/Portfolio_FullStack/`. All image, media, and resume URLs use that base. GitHub Pages publishes the committed `docs/` folder from `main`. After changing the site, rebuild with the command above and copy `dist/client/` into `docs/` before pushing. Keep `docs/.nojekyll` in place.

## Edit content

- `src/projects.js`: featured case studies, media captions, architecture descriptions, and source links.
- `src/App.jsx`: introduction, archive, biography, skills, contact, and dialog/gallery behavior.
- `src/styles.css`: typography, spacing, color tokens, and responsive layouts.
- `public/images/`: original project previews, optimized for the web.
- `public/media/ollama-demo.mp4`: compressed copy of the original classroom demonstration.
- `public/Maia-Arrais-Resume.pdf`: updated application resume.

Keep original project scope and contribution accurate when editing. Add measured results only when a method and supporting evidence are available. The portfolio presents academic and experimental prototypes; it does not imply aircraft experience or production deployment.

See [PORTFOLIO_GUIDE.md](PORTFOLIO_GUIDE.md) for content rationale, evidence sources, and useful additions before the application. See [MEDIA_SOURCES.md](MEDIA_SOURCES.md) for image and video provenance.

## Live portfolio

https://maiaarrais.github.io/Portfolio_FullStack/
