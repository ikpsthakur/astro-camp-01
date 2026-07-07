# Repository Guidelines

## Project Structure & Module Organization

This repository is currently a minimal starter workspace. Add source code under a clear top-level directory such as `src/`, tests under `tests/` or colocated as `*.test.*`, and static assets under `assets/` or `public/` depending on the framework selected. Keep generated output in ignored directories such as `dist/`, `build/`, or `.cache/`.

Use predictable module boundaries. For example, shared utilities belong in `src/lib/`, UI components in `src/components/`, and executable entry points in `src/main.*` or framework-specific route directories.

## Build, Test, and Development Commands

No package manifest or build tool is present yet. When tooling is introduced, document the primary commands here and keep them runnable from the repository root.

Common examples:

- `npm install`: install JavaScript dependencies when a `package.json` exists.
- `npm run dev`: start the local development server.
- `npm test`: run the test suite.
- `npm run build`: create a production build.

Prefer standard command names so contributors can discover workflows quickly.

## Coding Style & Naming Conventions

Follow the formatter and linter configured by the project once they exist. Until then, use 2-space indentation for JavaScript, TypeScript, JSON, YAML, Markdown, HTML, and CSS. Keep filenames lowercase and descriptive; use kebab-case for general files such as `user-card.tsx` and PascalCase only when required by a framework convention.

Keep functions small, name behavior explicitly, and avoid broad utility modules that mix unrelated concerns.

## Testing Guidelines

Add tests with each behavioral change. Name tests after the unit or feature being verified, for example `src/lib/date-format.test.ts` or `tests/login-flow.spec.ts`. Keep fast unit tests separate from slower integration or browser tests where possible.

When test tooling is added, make `npm test` or the equivalent command run the default suite without extra setup.

## Commit & Pull Request Guidelines

This workspace has no readable Git history, so no existing commit convention can be inferred. Use short, imperative commit messages such as `Add user profile route` or `Fix build config`.

Pull requests should include a concise summary, testing performed, linked issues when applicable, and screenshots for UI changes. Call out migrations, configuration changes, or breaking behavior explicitly.

## Agent-Specific Instructions

Respond to reasoning questions with brief responses. Before editing, inspect the repository and preserve user changes. Do not invent dependencies, commands, or conventions that are not represented in the project.
