# AGENTS.md

## Cursor Cloud specific instructions

This is a **content-only repository** (AI Whispers) — a curated collection of AI/LLM prompt engineering templates. It contains only Markdown files and a LICENSE; there is no executable code, no package manager, no build system, no automated tests, and no CI/CD.

### Key facts

- **44 Markdown files** organized into thematic directories (SCRUM, RPG, Prompt Improvement, etc.).
- Each prompt directory typically has a `readme.md` (explanation) and a `system.md` (the actual prompt template).
- No dependencies to install. The update script is a no-op (`echo` command).

### Linting

- `markdownlint-cli2` is installed globally via npm.
- Run `markdownlint-cli2 "**/*.md"` from the repo root to lint all Markdown files.
- The repository has pre-existing lint warnings (mostly line-length and formatting style). These are in the original content and are not regressions.

### Previewing content locally

- `grip` (GitHub Readme Instant Preview) is installed via pip.
- Run `grip README.md 0.0.0.0:8080` from the repo root to serve rendered Markdown at `http://localhost:8080/`.
- Subdirectory files are accessible by path, e.g. `http://localhost:8080/TreeOfThought/readme.md`.
- `grip` requires internet access on first run to download GitHub CSS; cached thereafter in `~/.grip/cache-*`.
