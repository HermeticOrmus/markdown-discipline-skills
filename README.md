<p align="center">
  <img src="https://ormus.solutions/mascot/chain_braces_to_swan.gif" alt="Markdown Discipline Skills" width="128" style="image-rendering: pixelated;" />
</p>

<h1 align="center">Markdown Discipline Skills</h1>

<p align="center">
  <em>A CLAUDE.md that strips AI-slop from markdown — no em dashes, no marketing fluff, no emoji bullets, sentence case headings. Anti-AI-tells discipline for any AI-assisted writing.</em>
</p>

<p align="center">
  <a href="https://github.com/HermeticOrmus/markdown-discipline-skills/stargazers"><img src="https://img.shields.io/github/stars/HermeticOrmus/markdown-discipline-skills?style=flat-square&color=aa8142" alt="Stars" /></a>
  <a href="https://github.com/HermeticOrmus/markdown-discipline-skills/blob/main/LICENSE"><img src="https://img.shields.io/github/license/HermeticOrmus/markdown-discipline-skills?style=flat-square&color=aa8142" alt="License" /></a>
  <a href="https://github.com/HermeticOrmus/markdown-discipline-skills/commits"><img src="https://img.shields.io/github/last-commit/HermeticOrmus/markdown-discipline-skills?style=flat-square&color=aa8142" alt="Last Commit" /></a>
  <img src="https://img.shields.io/badge/Claude_Code-aa8142?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code" />
</p>

---

> **A single `CLAUDE.md` that strips AI-slop from markdown. No em dashes, no marketing fluff, no emoji bullets, no triple-cataloging, no soft closes.**

## The problem

AI-generated documentation has tells. The em dash everywhere. The "powerful, comprehensive, world-class" adjective stack. The 🎉 Welcome banners. The "It's not X; it's Y" antithesis. The triple-bullet "fast, simple, reliable" cataloging. Soft closes like "Hope this helps!"

Once you can see the tells, you can't unsee them. AI docs read as AI docs. They are diluted by patterns the AI defaults to under load. They are longer than they need to be. They communicate less than they appear to.

## The solution

A `CLAUDE.md` file that bans the tells and codifies the discipline. Drop it into any project; Claude Code applies it to all markdown it writes for that project.

## What it covers

| Category | Discipline |
|---|---|
| Emoji | None unless asked — no headings, bullets, dividers, decorations |
| Marketing fluff | Strip "robust", "powerful", "leverage", "seamless", "world-class", "supercharge" |
| Heading style | Sentence case, one H1 per file, describe what's below not announce |
| Lists | One sentence per bullet, max 2 nesting levels |
| Code blocks | Always specify language, inline code for identifiers |
| Linking | Descriptive link text, relative paths, bare URLs only when URL is the content |
| Tables | 3+ items × 2+ dimensions; otherwise use a list |
| Em dash | Sparingly — common AI-tell when overused |
| Anti-patterns | Triple-cataloging, antithesis, clipped fragments, soft closes |

Full content: [`CLAUDE.md`](CLAUDE.md). Worked before/after examples: [`EXAMPLES.md`](EXAMPLES.md).

## Install

### As a project CLAUDE.md

Drop [`CLAUDE.md`](CLAUDE.md) at the root of your repository.

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/HermeticOrmus/markdown-discipline-skills/main/CLAUDE.md
```

If your project already has a CLAUDE.md, merge or append.

### As a Claude Code skill

The same content as an installable skill: [`skills/markdown-discipline/`](skills/markdown-discipline/).

### In Cursor

See [`CURSOR.md`](CURSOR.md). Rule at [`.cursor/rules/markdown-discipline.mdc`](.cursor/rules/markdown-discipline.mdc).

## Why this exists

LLMs have defaults. Under load — when generating prose, when writing READMEs, when documenting code — they fall back to defaults that are over-decorated and under-substantive. Strong defaults trained from a corpus heavy on marketing-style English will produce marketing-style English unless something tells them not to.

This file is that something.

## The reading test

For any paragraph you wrote (or the AI wrote for you), ask: did I learn anything new from the second half that wasn't in the first? If no, cut the second half.

For any list of three: are these three actually distinct things, or are they synonyms padded for rhythm? If padded, cut to one.

For any heading: does it tell me what's in the section, or does it announce that there's a section? "Authentication" beats "How Authentication Works."

For any sentence with an em dash: would a comma work? If yes, use the comma.

## What disciplined markdown looks like

Compare:

> ## 🎯 Why You'll Love This
>
> Our comprehensive, world-class CLAUDE.md empowers developers to write clean, professional, and effective documentation. It's not just a style guide — it's a powerful tool that transforms how teams collaborate. Fast. Simple. Reliable.

vs:

> ## What this fixes
>
> AI-generated markdown has predictable tells. This file lists them and bans them. The result reads like a human wrote it.

The second is shorter, denser, and tells you what's going to happen. That's the discipline.

## See also

- [`andrej-karpathy-skills`](https://github.com/HermeticOrmus/andrej-karpathy-skills) — companion: how Claude should behave when writing CODE (Karpathy's principles)
- [`vibe-engineer-skills`](https://github.com/HermeticOrmus/vibe-engineer-skills) — companion: how YOU should behave when directing Claude

## Contributing

PRs welcome — especially for additional AI-tell patterns I haven't named yet (you'll know them when you see them), translations of the README, and adaptations of CURSOR.md for other AI tools.

## License

MIT.

---

## Part of the Libre Open-Source Stack for Claude Code

This repository is part of a growing family of open-source toolkits for Claude Code.

### Libre suite — comprehensive plugin bundles

- [LibreUIUX-Claude-Code](https://github.com/HermeticOrmus/LibreUIUX-Claude-Code) — UI/UX development (152 agents, 70 plugins, 76 commands, 74 skills)
- [LibreArch-Claude-Code](https://github.com/HermeticOrmus/LibreArch-Claude-Code) — Software architecture and system design
- [LibreCopy-Claude-Code](https://github.com/HermeticOrmus/LibreCopy-Claude-Code) — Technical writing and documentation engineering
- [LibreDevOps-Claude-Code](https://github.com/HermeticOrmus/LibreDevOps-Claude-Code) — DevOps engineering and infrastructure automation
- [LibreEmbed-Claude-Code](https://github.com/HermeticOrmus/LibreEmbed-Claude-Code) — Embedded systems, firmware, and IoT development
- [LibreFinTech-Claude-Code](https://github.com/HermeticOrmus/LibreFinTech-Claude-Code) — Financial technology development
- [LibreGEO-Claude-Code](https://github.com/HermeticOrmus/LibreGEO-Claude-Code) — AI-search optimization (ChatGPT, Perplexity, Gemini, Google AI Overviews)
- [LibreGameDev-Claude-Code](https://github.com/HermeticOrmus/LibreGameDev-Claude-Code) — Game development across Godot, Unity, Unreal
- [LibreMLOps-Claude-Code](https://github.com/HermeticOrmus/LibreMLOps-Claude-Code) — ML engineering and AI operations
- [LibreMobileDev-Claude-Code](https://github.com/HermeticOrmus/LibreMobileDev-Claude-Code) — Mobile app development (Flutter, React Native, native iOS, native Android)
- [LibreSecOps-Claude-Code](https://github.com/HermeticOrmus/LibreSecOps-Claude-Code) — Security operations
- [LibreSessionFlow-Claude-Code](https://github.com/HermeticOrmus/LibreSessionFlow-Claude-Code) — Session lifecycle: handoff, pickup, absorb, explore, close

### Skills mini-repos — single CLAUDE.md drop-ins

- [vibe-engineer-skills](https://github.com/HermeticOrmus/vibe-engineer-skills) — Direct AI codegen well: hypothesis before help, scoped prompts, validate before accepting
- [shell-safety-skills](https://github.com/HermeticOrmus/shell-safety-skills) — `set -euo pipefail` discipline plus 15 failure-mode examples
- [commit-standard-skills](https://github.com/HermeticOrmus/commit-standard-skills) — Ormus Commit Standard v1.0 plus commit-msg hook and commitlint
- [unwoke-skills](https://github.com/HermeticOrmus/unwoke-skills) — Strip AI theater (ten sins to eliminate, symmetric engagement)
- [python-conventions-skills](https://github.com/HermeticOrmus/python-conventions-skills) — Modern Python 3.11+ (types, pathlib, async, ruff, mypy, uv)
- [typescript-conventions-skills](https://github.com/HermeticOrmus/typescript-conventions-skills) — TypeScript strict mode, discriminated unions, Result types
- [hermetic-laws-skills](https://github.com/HermeticOrmus/hermetic-laws-skills) — Seven Hermetic Principles applied to engineering
- [riper-workflow-skills](https://github.com/HermeticOrmus/riper-workflow-skills) — Research / Innovate / Plan / Execute / Review systematic dev
- [six-day-cycle-skills](https://github.com/HermeticOrmus/six-day-cycle-skills) — Sustainable shipping cadence with mandatory rest
- [token-optimization-skills](https://github.com/HermeticOrmus/token-optimization-skills) — Claude Code token and context optimization
- [osint-skills](https://github.com/HermeticOrmus/osint-skills) — OSINT research methodology (multi-wave investigative spiral)
- [calcinate-skills](https://github.com/HermeticOrmus/calcinate-skills) — Stage 1 of the Magnum Opus (burn project bloat)
- [claude-md-overhaul-skills](https://github.com/HermeticOrmus/claude-md-overhaul-skills) — Audit CLAUDE.md and MEMORY.md against caps
- [session-handoff-skills](https://github.com/HermeticOrmus/session-handoff-skills) — Session handoff and pickup discipline
- [naming-skills](https://github.com/HermeticOrmus/naming-skills) — Product naming methodology (mine the brand's vocabulary)
- [magnum-opus-skills](https://github.com/HermeticOrmus/magnum-opus-skills) — Seven-stage alchemy applied to project transformation
- [mem-search-skills](https://github.com/HermeticOrmus/mem-search-skills) — Search claude-mem cross-session memory: search, filter, fetch
- [hypothesis-debugging-skills](https://github.com/HermeticOrmus/hypothesis-debugging-skills) — Hypothesis-driven debugging: reproduce, isolate, test, fix
- [vibe-proof-skills](https://github.com/HermeticOrmus/vibe-proof-skills) — Security hardening for vibe-coded full-stack apps
- [tdd-skills](https://github.com/HermeticOrmus/tdd-skills) — Test-driven development (Red-Green-Refactor) for JS/TS and Python
- [mars-skills](https://github.com/HermeticOrmus/mars-skills) — Production-readiness audit: the five mortal sins of vibe-coded MVPs
- [git-workflow-skills](https://github.com/HermeticOrmus/git-workflow-skills) — Clean git workflow: branch, atomic commits, reviewable PRs
- [code-review-skills](https://github.com/HermeticOrmus/code-review-skills) — Domain-aware code review: classify the code, then focus
- [explore-code-skills](https://github.com/HermeticOrmus/explore-code-skills) — Understand an unfamiliar codebase fast
- [dx-audit-skills](https://github.com/HermeticOrmus/dx-audit-skills) — Audit developer experience: docs, onboarding, tooling friction
- [setup-env-skills](https://github.com/HermeticOrmus/setup-env-skills) — Set up a project's development environment
- [automate-skills](https://github.com/HermeticOrmus/automate-skills) — Turn repetitive tasks into reliable automation scripts
- [quick-fix-skills](https://github.com/HermeticOrmus/quick-fix-skills) — Fast troubleshooting for common issues
- [prime-context-skills](https://github.com/HermeticOrmus/prime-context-skills) — Prime project context at the start of a session
- [auto-docs-skills](https://github.com/HermeticOrmus/auto-docs-skills) — Generate and maintain project documentation
- [learning-skills](https://github.com/HermeticOrmus/learning-skills) — Learn any technology: roadmaps, explanations, practice, cheatsheets, comparisons
- [linux-sysadmin-skills](https://github.com/HermeticOrmus/linux-sysadmin-skills) — Linux system administration: security, performance, diagnostics, monitoring, maintenance

### Template source

- [andrej-karpathy-skills](https://github.com/HermeticOrmus/andrej-karpathy-skills) — the canonical single-file CLAUDE.md pattern (fork of jiayuan_jy's original)

Star the family, not just one — that's how the suite stays coherent.
