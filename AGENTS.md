# AGENTS.md

## Cursor Cloud specific instructions

This is a **content-only Markdown repository** (AI Whispers) — a curated collection of AI/LLM system prompts. There is no application code, no build system, no automated test suite, and no services to run.

### Repository structure

- Each subdirectory contains a prompt with `system.md` (the prompt text) and `readme.md` (documentation/background).
- Prompt categories: SCRUM assistants, text processing, RPG/TTRPG tools, metaprompts, PanelGPT variations, Tree of Thought, etc.
- Root files: `README.md` (index of all prompts), `LICENSE` (GPL v3).

### Development workflow

- **Lint**: `markdownlint-cli2 "**/*.md"` — validates all Markdown files. Existing files have pre-existing style issues (719 as of initial setup); new/edited files should aim for clean lint.
- **Preview**: `marked` CLI is available globally for rendering Markdown to HTML (e.g., `marked -i TreeOfThought/system.md`).
- **No build/test/run step**: There are no compile, build, or test commands since the repo is pure Markdown content.
