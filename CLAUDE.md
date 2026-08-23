# Claude Code Documentation Mirror

This repository contains local copies of Claude Code documentation from https://docs.anthropic.com/en/docs/claude-code/

The docs are periodically updated via GitHub Actions.

## For /docs Command

When responding to /docs commands:
1. Follow the instructions in the docs.md command file
2. Read documentation files from the docs/ directory only
3. Use the manifest to know available topics

## Key files

Read these on demand — do not preload them. They are listed here so you know
where to look, not so their contents sit in context every session.

- `install.sh` — installer / migrator (v0.3.3), sets up `/docs` command + PreToolUse hook
- `uninstall.sh` — smart uninstaller, finds installs from configs
- `UNINSTALL.md` — manual uninstall instructions
- `README.md` — user-facing docs, usage examples, troubleshooting
- `scripts/claude-docs-helper.sh.template` — source of the `/docs` helper script
- `scripts/fetch_claude_docs.py` — scraper that pulls docs from docs.anthropic.com
- `.github/workflows/update-docs.yml` — scheduled sync job (every 3 hours)
- `docs/` — the mirrored documentation (~40 files)
- `docs/docs_manifest.json` — index of available topics; tracked by git, never edit manually
