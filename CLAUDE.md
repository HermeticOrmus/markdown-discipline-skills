# CLAUDE.md

Behavioral guidelines for markdown writing — strip the AI-slop tells, leave the signal. Apply to docs, READMEs, briefs, and any markdown content. The goal: high-signal text that reads well as both a doc and as context for an LLM.

**Tradeoff**: bias toward direct over decorated. For creative writing or marketing copy where flourish is intentional, use judgment.

## No emojis unless asked

The user explicitly does not want emojis in files. Not in headings. Not as bullet markers. Not as section dividers. Not as decoration around important text. If the user asks for emojis, that's the override.

## No marketing fluff

These words and patterns are AI-tells that signal lack of substance. Strip them:

- **Adjectives**: "robust", "powerful", "comprehensive", "seamless", "world-class", "best-in-class", "cutting-edge", "innovative", "revolutionary"
- **Verbs**: "leverage" (as a verb), "unleash", "supercharge", "elevate", "transform"
- **Greetings**: "🎉 Welcome!", "✨ Get started!", "🚀 Let's dive in!"
- **Conclusions**: "In summary,", "To wrap up,", "In conclusion,", "Hope this helps!"
- **Hedging**: "It's worth noting that", "It's important to remember", "Keep in mind that"

Lead with what it does, not how great it is.

## Heading style

- **Sentence case** for headings, not Title Case. `## Why this exists`, not `## Why This Exists`.
- One `#` per file (the title). Use `##` and `###` for sections.
- Headings describe what's BELOW them, not announce them. `## Configuration`, not `## How to Configure`.
- No emoji in headings. No badges in headings.

## Lists

- Bullets when order doesn't matter, numbered when it does.
- One sentence per bullet ideally. If the bullet needs a paragraph, it shouldn't be a bullet.
- Don't sub-nest bullets more than 2 levels deep. If you need more, restructure.
- Don't use bullets for connected prose — use paragraphs.

## Code blocks

- Always specify language for syntax highlighting: ` ```bash`, ` ```ts`, ` ```python`.
- Inline code for: filenames, env vars, command names, function names, type names.
- Block code for anything multi-line, or for clarity even if a single line.

## Linking

- `[link text](url)` — make link text describe the destination, not "click here".
- Relative paths for in-repo links so they survive file moves.
- Bare URLs only when the URL itself IS the content (e.g., a citation).

## Tables

- Use when comparing 3+ items across 2+ dimensions.
- Don't use for what's really a list with annotations — a list reads cleaner.
- Keep cells short. If a cell needs a paragraph, it doesn't belong in a table.

## Em dash and en dash

- Em dash `—` reads as an AI-tell when it appears more than once or twice per page. Use sparingly.
- En dash `–` for ranges (`pages 12–15`) and never as a substitute for em dash.
- Prefer commas or periods where an em dash would be optional.

## AI-tell anti-patterns to strip

- **Triple-cataloging**: "fast, simple, and reliable" or "powerful, flexible, and intuitive" — three adjectives chained that the AI defaults to.
- **Antithesis**: "It's not X; it's Y" — the AI's favorite rhetorical move.
- **Clever metaphors**: "Think of it as a thermostat for your codebase" — clever metaphors that don't actually clarify.
- **Clipped fragments**: "Fast. Reliable. Powerful." — sentence fragments for emphasis, the LinkedIn style.
- **Soft closes**: "Hope this helps!" or "Let me know if you have questions!"
- **Self-references**: "As mentioned above" or "We discussed earlier" — say it once, in the right place.

## Anti-patterns in formatting

- Emoji bullets / dividers / section breaks
- Marketing adjectives in technical docs
- Title Case headings
- Excessive bold for emphasis (one bolded phrase per paragraph max)
- Block quotes used as fancy callouts (use them only for actual quotations)
- Trailing whitespace at line ends
- Mixing `-` and `*` for bullets in the same file
- Multiple H1s in one file (multiple `#` headings)

## What good markdown reads like

The same content, before and after:

**Before** (AI-slop):
> # 🚀 Getting Started with Our Powerful API
>
> Welcome! Our comprehensive, world-class API empowers developers to build seamless, scalable applications. Let's dive in! 🎉
>
> ## ✨ Quick Start
>
> Getting up and running is fast, simple, and reliable. Here's how to leverage our robust authentication system:

**After** (disciplined):
> # API quickstart
>
> Authenticate, make your first request, parse the response.
>
> ## Authenticate
>
> The API uses bearer tokens. Get one at the dashboard, then:

The disciplined version is shorter, denser, and tells you what's actually going to happen.

---

**License**: MIT — use it, fork it, merge it into your own.
