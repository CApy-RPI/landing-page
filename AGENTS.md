# Repository Guidelines

## Project Structure & Module Organization
The root directory holds the static pages (`index.html`, `features.html`, `changelog.html`, `about.html`, `contact.html`) alongside page-specific stylesheets such as `homepage.css` and `about.css`. Shared layout rules live in `head_foot.css`, while all imagery is stored in `images/`. Keep new assets in that folder and reference them with relative paths. When adding a new page, pair it with a dedicated stylesheet and reuse the shared header/footer markup to maintain navigation consistency.

## Build, Test, and Development Commands
This project ships as pure HTML/CSS, so no build step is required. For a local preview, run `python3 -m http.server 8000` from the repository root and open `http://localhost:8000/index.html`. Use the browser’s developer tools to test responsive layouts; no additional tooling is expected.

## Coding Style & Naming Conventions
Follow the existing four-space indentation in HTML and CSS. Keep HTML attributes ordered consistently (`href`, `id`, `class`) and favor semantic tags where practical. Name new stylesheets and IDs in lower-case with underscores only when needed; prefer descriptive hyphenated class names (e.g., `.feature-card`). Reuse shared color variables and animations by extending the rules already present in `head_foot.css` and the page-specific files.

## Testing Guidelines
There are no automated tests today; rely on manual verification. Confirm that every navigation link works, check for obvious layout regressions on desktop and mobile breakpoints, and validate that external embeds (fonts, icons) still load. Document the browsers you exercised and any responsive viewports you inspected when submitting changes.

## Commit & Pull Request Guidelines
Use short, imperative commit messages similar to the existing history (e.g., `[Update] - Refresh homepage hero`). Group related edits into a single commit when possible. Pull requests should include a summary of the pages touched, screenshots or recordings for UI changes, and references to any related issues. Mention any manual testing performed so reviewers can reproduce it quickly.
