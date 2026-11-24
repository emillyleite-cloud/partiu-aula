# Repository Guidelines

## Project Structure & Module Organization

This workspace currently contains project reference material only. `Docs/requirements (1).md` describes the Partiu Aula student ride-sharing app, its requirements, and usability goals. `Docs/1.png` through `Docs/4.png` are visual references. There is no application source code, test suite, or asset pipeline in the current tree. If implementation is added, keep production code and tests in clearly named directories (for example, `src/` and `tests/`) and keep design references in `Docs/`.

## Build, Test, and Development Commands

No build, test, or local-run commands are defined in this workspace. When adding an application, document its actual setup and commands here and in the relevant project README; do not commit commands that have not been verified for the chosen toolchain.

## Coding Style & Naming Conventions

No language or formatter is established yet. Follow the conventions of the framework selected for implementation, use consistent formatting, and choose descriptive names that reflect the ride-sharing domain (for example, `RideOffer` and `bookingStatus`). Keep user-facing messages clear and provide actionable validation feedback, as required by the project brief.

## Testing Guidelines

There is no test framework or coverage requirement yet. Add tests alongside new functionality using the chosen framework's standard naming pattern, and document how contributors can run them. Prioritize core flows from the requirements: account access, ride search and offers, reservation status, messaging, and post-trip ratings.

## Commit & Pull Request Guidelines

Git history is not available in this workspace, so no established commit convention can be confirmed. Use short, imperative commit subjects (for example, `Add ride search screen`). Pull requests should explain the user-facing change, list relevant checks, link related work when applicable, and include screenshots for interface changes.

## Security & Configuration

Do not commit credentials, private user information, or production secrets. Keep local configuration in ignored environment files and provide a sanitized example if implementation requires configuration.