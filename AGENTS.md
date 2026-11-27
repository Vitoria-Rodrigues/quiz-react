# Quiz React Agents Context

This document serves as the sovereign root context router (Layer 1) for AI agents operating in the `Vitoria-Rodrigues/quiz-react` repository.

## Navigation

- [README.md](./README.md): Primary developer documentation, state-machine diagram, and pnpm setup guide.
- [.agents/plugins.json](./.agents/plugins.json): Antigravity plugin registry importing domain plugins from `@vitoria-rodrigues/agent-mesh`.
- [pnpm-workspace.yaml](./pnpm-workspace.yaml): Centralized dependency catalogs (`catalogMode: strict`) and `@vitoria-rodrigues/agent-mesh` registration.
- [package.json](./package.json): Scoped package manifest (`@vitoria-rodrigues/quiz-react`) and Vite scripts.

## Architecture

The application is an interactive programming trivia SPA built with React 19, Vite 7, and React Context API:

- **`src/context/quiz.jsx`**: Central `QuizContext` provider and `quizReducer` state machine transitioning across `Start`, `Category`, `Playing`, and `End`.
- **`src/data/`**: Categorized trivia question banks (`questions.js`, `questions_complete.js`) for HTML, CSS, and JavaScript.
- **`src/components/`**: Modular views (`Welcome.jsx`, `PickCategory.jsx`, `Question.jsx`, `Option.jsx`, `GameOver.jsx`) with dedicated CSS files.
- **`src/img/`**: SVG illustrations for game stages (`quiz.svg`, `category.svg`, `welldone.svg`).

## Scoped Guardrails

- MUST maintain a strict senior, objective, and technical tone across all communications, documentation, and code.
- MUST conduct conversational chat responses in Brazilian Portuguese (pt-BR) while keeping all code, configuration files, commit messages, and technical documentation in English (en-US).
- MUST NOT use emojis anywhere in code, markdown headers, body text, commit messages, or chat responses (Zero-Emoji Invariant).
- MUST use `pnpm` exclusively and consume all dependencies via `catalog:` entries in `pnpm-workspace.yaml` (never raw semver strings in `package.json`).
- MUST consume `@vitoria-rodrigues/agent-mesh` solely via `catalog:plugins-stack` and `.agents/plugins.json` without storing legacy plugins, skills, or docs inside `.agents/`.
- MUST use Conventional Commits v1.0.0 (`<type>(<scope>): <description>`) and sign commits with SSH (`git commit -S -m "..."`) when `user.signingkey` is configured.
- MUST use relative paths for all Markdown links inside repository files.

## Required Skills

When operating in this repository, agents MUST activate the relevant `@vitoria-rodrigues/agent-mesh` skill:

- **`router-architect`**: Active when authoring or auditing `AGENTS.md` context routers.
- **`readme-architect`**: Active when updating or auditing `README.md` documentation.
- **`monorepo-architect`**: Active when auditing `pnpm-workspace.yaml` catalogs or `package.json` manifests.
- **`github-flow-operator`**: Active when creating branches, commits, or pull requests.
