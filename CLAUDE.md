# Claude Code Documentation Mirror

This repository contains local copies of Claude Code documentation from https://docs.anthropic.com/en/docs/claude-code/

The docs are periodically updated via GitHub Actions.

## For /docs Command

When responding to /docs commands:
1. Follow the instructions in the docs.md command file
2. Read documentation files from the docs/ directory only
3. Use the manifest to know available topics

## Key files (read on demand, don't preload)
- `install.sh` — installer/migrator, v0.3.3
- `uninstall.sh` — smart uninstaller
- `scripts/claude-docs-helper.sh.template` — the /docs helper
- `scripts/fetch_claude_docs.py` — doc scraper
- `.github/workflows/update-docs.yml` — 3-hour sync job
