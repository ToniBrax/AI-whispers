## Cursor Cloud specific instructions

This repository (**AI Whispers**) is a documentation-only collection of AI/LLM prompt templates stored as Markdown files. It contains **no source code, no build system, no tests, no dependencies, and no services**.

### Repository structure

- Each prompt has its own directory (e.g. `TreeOfThought/`, `PanelGPT/`, `RPG - AIMS/`)
- Each directory typically contains a `readme.md` (explanation/background) and a `system.md` (the prompt text)
- Two standalone prompts live at root level: `contextual scaffolding.md` and `program simulation framework.md`
- `README.md` at root is the main index with links to all prompts

### Development notes

- **No build/lint/test commands exist.** There is no `package.json`, `Makefile`, or any build tooling.
- **No services to start.** The content is static Markdown meant to be read or copy-pasted into LLM interfaces.
- **No dependencies to install.** The update script is intentionally a no-op.
- To validate content integrity, verify all `.md` files are readable: `find . -name "*.md" -not -path "./.git/*" -exec wc -l {} +`
