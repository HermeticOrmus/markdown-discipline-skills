# Using this repo with Cursor

This project includes a **Cursor project rule** so the markdown discipline applies automatically when you work here.

## In this repository

1. Open the folder in Cursor.
2. The rule [`.cursor/rules/markdown-discipline.mdc`](.cursor/rules/markdown-discipline.mdc) is committed with `alwaysApply: true`.
3. Confirm under Cursor **Settings → Rules**.

## Use the same discipline in another project

**Cursor**: Copy `.cursor/rules/markdown-discipline.mdc` into that project's `.cursor/rules/` directory.

**Other AI tools**: Copy [`CLAUDE.md`](CLAUDE.md) to your project root. Most AI coding tools (Claude Code, Continue, Cline, Windsurf, Aider) read a root instruction file.

## Optional: personal skill

The same content as a reusable skill at [`skills/markdown-discipline/SKILL.md`](skills/markdown-discipline/SKILL.md). Copy or symlink into `~/.claude/skills/` or `~/.cursor/skills/`.
