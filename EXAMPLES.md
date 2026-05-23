# Examples

Before-and-after pairs for each category of the markdown discipline. The "before" is AI-default output; the "after" applies the discipline.

---

## 1. The marketing-banner opening

**Before**:
> # 🚀 Getting Started with Our Powerful API
>
> Welcome! Our comprehensive, world-class API empowers developers to build seamless, scalable applications. Let's dive in! 🎉

**After**:
> # API quickstart
>
> Authenticate, make your first request, parse the response.

**What changed**: removed emoji, marketing adjectives, the "Welcome" greeting, the "Let's dive in" call-out. Cut from 24 words to 9. The reader now knows what's coming.

---

## 2. Triple-cataloging

**Before**:
> Our library is fast, simple, and reliable. Built for developers who value performance, clarity, and stability.

**After**:
> The library is fast. Performance benchmarks at the bottom of the README.

**What changed**: dropped the synonyms cataloged for rhythm. Made the claim verifiable by pointing at the proof.

---

## 3. Antithesis

**Before**:
> It's not just a logger — it's a comprehensive observability solution.

**After**:
> It's a logger with span tracing and metric export built in.

**What changed**: stated what it is instead of staging a contrast with what it isn't. Specific features beat abstract category claims.

---

## 4. The clever metaphor

**Before**:
> Think of `useState` as a thermostat for your component's data — it senses, regulates, and adjusts as conditions change.

**After**:
> `useState` returns a value and a setter. Calling the setter re-renders the component with the new value.

**What changed**: dropped the metaphor (which didn't actually clarify), described the mechanism literally.

---

## 5. Title Case headings

**Before**:
> ## How To Configure The Database Connection
> ## Setting Up Your First Migration
> ## Running The Test Suite

**After**:
> ## Configure the database connection
> ## Run your first migration
> ## Run the test suite

**What changed**: sentence case throughout. Imperative mood ("Configure" not "How To Configure"). Read like instructions, not blog post titles.

---

## 6. Heading that announces instead of describes

**Before**:
> ## How Authentication Works in This System
>
> The authentication system uses JWT tokens. When a user logs in, ...

**After**:
> ## Authentication
>
> The authentication system uses JWT tokens. When a user logs in, ...

**What changed**: heading describes what's in the section. The body explains how.

---

## 7. Emoji bullets

**Before**:
> - ✅ Real-time updates
> - 🔒 End-to-end encryption
> - 📊 Built-in analytics
> - 🚀 Sub-100ms response times

**After**:
> - Real-time updates via WebSocket
> - End-to-end encryption with libsodium
> - Built-in analytics dashboard at `/admin`
> - Sub-100ms p95 response times

**What changed**: dropped the emoji decoration. Added the substance the emoji was substituting for. Now each bullet answers "how" or "where."

---

## 8. The soft close

**Before**:
> ## Conclusion
>
> Hope this helps! Let me know if you have any questions or run into issues. Happy coding! 🚀

**After**:
> *(no conclusion section)*

**What changed**: deleted. A good doc doesn't need a closing salutation; the last useful sentence IS the close. "Conclusion" sections that summarize what was just said dilute density.

---

## 9. Bullet overuse for prose

**Before**:
> - This feature is important because:
>   - It improves user experience
>   - It increases retention
>   - It is requested by enterprise customers
>   - It differentiates us from competitors
>   - It aligns with our product strategy

**After**:
> Enterprise customers asked for it; retention modeling supports it; we ship it in Q3.

**What changed**: prose where prose is natural; the bullets were padding what could be one sentence.

---

## 10. Hedging filler

**Before**:
> It's worth noting that the API endpoint is rate-limited. Keep in mind that exceeding the rate limit results in a 429 response. It's important to remember to implement exponential backoff in your retry logic.

**After**:
> The endpoint is rate-limited. Exceeding the limit returns 429. Use exponential backoff for retries.

**What changed**: removed "It's worth noting", "Keep in mind", "It's important to remember". Three sentences became three sentences each carrying actual information.

---

## 11. Excessive bold

**Before**:
> The **most important** thing to understand is that **state** is **immutable**. You **must** use the **setter function** to update it — **never** mutate state **directly**.

**After**:
> State is immutable. Use the setter to update it; never mutate directly.

**What changed**: bold was indicating which words the writer thought were important. Removed it. One bolded phrase per paragraph max — usually fewer.

---

## 12. Block quotes as callouts

**Before**:
> > **⚠️ Important!**
> >
> > Make sure to back up your database before running migrations.

**After**:
> Back up your database before running migrations.

**What changed**: block quote is for actual quotations. A warning is just a sentence; treat it like one. If urgency is needed, use position (top of section) and clarity, not formatting.

---

## 13. Em dash overuse

**Before**:
> The system — which is the foundation of our platform — provides real-time updates — across all clients — without polling.

**After**:
> The system provides real-time updates across all clients, without polling. It's the foundation of our platform.

**What changed**: em dashes are an AI-tell when overused. Used twice in one paragraph is too many. Used in lieu of commas or paragraph breaks is lazy. Use sparingly.

---

## 14. Clipped fragments

**Before**:
> Built for speed.
>
> Built for scale.
>
> Built for you.

**After**:
> Built for high-throughput, multi-tenant deployments. Specifically: > 100k req/sec p99 < 10ms.

**What changed**: clipped fragments are LinkedIn-style emphasis. They look like rhythm but communicate nothing specific. Replace with the specific claim.

---

## 15. Multiple H1s

**Before**:
> # Introduction
>
> ...
>
> # Installation
>
> ...
>
> # Usage
>
> ...

**After**:
> # Project Name
>
> ## Introduction
>
> ...
>
> ## Installation
>
> ...
>
> ## Usage

**What changed**: One `#` per file (the title). All sections are `##` or `###`. Tools that generate tables of contents from H1s rely on this.

---

## How to use this in practice

When you write markdown (or accept AI-generated markdown), scan for:

1. **Emoji** — anywhere
2. **Adjective stacks** — three adjectives in a row, especially marketing ones
3. **"It's not X; it's Y"** — the antithesis pattern
4. **Triple bullets** — three short bullets that catalog a single idea
5. **Soft closes** — "Hope this helps", "Let me know if"
6. **Bold scatter** — more than one bolded phrase per paragraph
7. **Em dash count** — more than 2 per page is suspicious
8. **Sentence fragments for emphasis** — "Fast. Simple. Reliable."

When you see any of them, edit. Each one cut is a signal-to-noise improvement.

## What this doesn't cover

This is style, not content. Disciplined markdown can still be wrong. A polished, em-dash-free, sentence-case README can still lie. Style is necessary, not sufficient.

For content discipline, see the [`vibe-engineer-skills`](https://github.com/HermeticOrmus/vibe-engineer-skills) and [`andrej-karpathy-skills`](https://github.com/HermeticOrmus/andrej-karpathy-skills) repos.
