# Repository Guidelines

## Project Structure & Module Organization
This repository is a small static site. The main entrypoint is [`index.html`](./index.html), styles live in [`styles.css`](./styles.css), and visual assets are stored under [`assets/`](./assets/). There is no JavaScript build layer or package manager metadata yet, so changes should stay consistent with this simple file layout.

## Build, Test, and Development Commands
There is no build step or automated test suite in the repository. Edit the files directly and preview the page in a browser. Useful local checks:

- `git status --short` to review modified files.
- Open `index.html` in a browser to verify layout, images, and responsive behavior.

If a dev server is introduced later, document it here and keep the command list current.

## Coding Style & Naming Conventions
Use two-space indentation in HTML and CSS, and keep files ASCII unless existing content requires otherwise. Prefer descriptive class names that match the page sections already in use, such as `hero`, `feature-card`, and `gallery-grid`. Keep CSS organized by layout first, then typography, then component styles, then media queries.

## Testing Guidelines
No test framework is configured. Manual verification should cover:

- Desktop and mobile viewport layout
- Image loading from `assets/`
- Anchor navigation between sections
- Readability of text over gradients and glassmorphism surfaces

When adding interactive behavior later, add a lightweight test or script and document how to run it.

## Commit & Pull Request Guidelines
The existing history uses short, direct commit messages; the initial commit is `初次生成`. Follow the same pattern: concise, imperative, and specific to the change. Pull requests should summarize the visual or structural change, mention any assets added or replaced, and include screenshots for layout updates.

## Agent Notes
Avoid introducing unnecessary tooling. Keep changes scoped to the static page unless the task explicitly requires more structure.
