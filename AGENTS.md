# Repository Guidelines

## Project Structure & Module Organization

This repository contains a static web MVP and project references for Partiu Aula, a student carpooling app. `index.html` defines the screens, `styles.css` contains responsive and accessible presentation styles, and `app.js` implements navigation and demo interactions. `docs/requirements.md` is the source of truth for project goals, user scenarios, and functional requirements; prototype screenshots belong in `docs/`.

## Build, Test, and Development Commands

The MVP has no build step or package dependencies. Open `index.html` in a modern browser to use it locally. For a local HTTP server, run `python -m http.server 8000` from the repository root, then visit `http://localhost:8000`. User-created offers and reservation requests are stored in browser `localStorage` for this demonstration.

## Documentation & Asset Conventions

Write documentation in Markdown with descriptive headings, short paragraphs, and tables for structured requirements. Keep requirement IDs stable (for example, `RF01`) when editing `docs/requirements.md`, and update related scenarios or acceptance criteria when behavior changes. Use clear, descriptive filenames for new assets, such as `prototype-home.png`; avoid timestamp-only names when adding new material. Keep screenshots and prototype exports in `docs/` and link to them with relative paths.

## Testing Guidelines

There is no automated test framework or coverage target at present. When changing the MVP, manually check the main navigation, search and sorting, ride details and reservation, offer validation and publishing, mobile layout, and keyboard focus. For documentation changes, check Markdown links, requirement references, and asset paths. Add a test framework only when the project adopts one, and document its command here.

## Commit & Pull Request Guidelines

Git history is not available in this workspace, so no existing commit message convention can be confirmed. Use concise imperative commit subjects that describe one change (for example, `Document ride request flow`). Pull requests should explain the user-facing or documentation change, list affected requirements or files, link related work when available, and include screenshots for visual updates. Note any checks performed and any follow-up work.

## Scope & Configuration

The requirements document intentionally leaves implementation technology and integrations undecided. Confirm proposed technical decisions against the product requirements and record them in the repository before relying on them. Do not commit credentials, personal data, or local environment files.
