# Markdown Discipline Skills

> A single `CLAUDE.md` that strips AI-slop from markdown. No em dashes, no marketing fluff, no emoji bullets, no triple-cataloging, no soft closes.

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
