<!-- Import workspace-level CLAUDE.md configuration -->
<!-- See /home/lab/workspace/.claude/CLAUDE.md for complete rules -->

# Project-Specific Configuration

This file extends workspace-level configuration with project-specific rules.

## Project Context

**jupyterlab_close_all_tabs_extension** - A JupyterLab 4 extension that adds a "Close All Tabs" menu item under the Tabs menu, allowing users to close all open tabs with a confirmation dialog.

## Technology Stack

- **Frontend**: TypeScript, JupyterLab 4 extension API
- **Build**: jlpm (JupyterLab's yarn), webpack via @jupyterlab/builder
- **Python packaging**: hatchling, hatch-jupyter-builder
- **Testing**: Jest (unit), Playwright/Galata (integration)
- **Linting**: ESLint, Prettier, Stylelint

## Package Details

- **npm**: `jupyterlab_close_all_tabs_extension`
- **PyPI**: `jupyterlab-close-all-tabs-extension`
- **Repository**: github.com/stellarshenson/jupyterlab_close_all_tabs_extension

## Key Files

- `src/index.ts` - Main extension plugin
- `package.json` - npm configuration, version source
- `pyproject.toml` - Python build configuration
- `jupyterlab_close_all_tabs_extension/` - Python package with labextension

## Build Commands

```bash
jlpm build        # Development build
jlpm build:prod   # Production build
jlpm test         # Run Jest tests
jlpm lint         # Run all linters
jlpm watch        # Watch mode for development
```
