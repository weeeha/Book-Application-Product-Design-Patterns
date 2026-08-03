# Application Product Design Patterns — Design Spec

**Date:** 2026-08-02 · **Status:** Draft for author review · **Author:** Nick Vyhouski (brainstormed with Claude)

## What this is

A public web book of product-design patterns for complex web applications, written from Nick's 14+ years and 20+ shipped products. Working title: **Application Product Design Patterns** (public brand name chosen at launch, not before).

## Goals, priority-ordered

1. **Authority** — a citable, linkable body of work that positions Nick at Staff/Principal level. When goals conflict, this wins; the book stays free and public.
2. **Teach** — genuinely useful to its readers, not a portfolio in disguise.
3. **Systematize** — extract and structure the patterns Nick actually uses.
4. **Sellable later** — source format must allow PDF/EPUB export eventually; never at the cost of goals 1–3.

## Audience

Primary readers are **founders, PMs, and AI-era builders** — people shipping complex web apps without a design team, whether they brief a designer or prompt an AI coding tool.

Implications:
- Written at **decision altitude**: when the pattern applies, what it costs, what breaks without it — not pixel-craft instruction.
- Plain business vocabulary; design jargon only when it earns its place.
- Every pattern ends with a section on getting the pattern out of an AI coding tool correctly.

## Spine and scope

- Spine: **the recurring surfaces and decisions of B2B SaaS web apps**, with **AI product patterns as a major section**.
- v1 = **any 8 of the 12 candidate patterns live** at the unlisted URL, **at least 2 of them from the AI section** (so v1 keeps the AI promise). The book grows pattern by pattern after that.
- Explicitly not in v1: e-book export, custom domain, newsletter/comments, CMS, print.

## Pattern anatomy (every chapter, same six blocks)

1. **The situation** — the moment a builder hits this wall, in plain language.
2. **Forces** — what is actually in tension; why the obvious fix fails.
3. **The pattern** — what to do, with annotated visuals.
4. **From the field** — the real story from Nick's shipped work.
5. **Anti-patterns** — the two or three ways teams get it wrong.
6. **Build it with AI** — how to brief an AI coding tool to produce this correctly.

## v1 candidate patterns

| # | Pattern | Field evidence |
|---|---------|----------------|
| 1 | The "is everything OK?" dashboard — status before charts | BindPlane, SelectStar, Ten8 |
| 2 | Data tables that survive real data | Pendo Data Explorer, Acies.ai |
| 3 | Drill-down without losing context | Acies.ai, Data Plus Math |
| 4 | The adaptive wizard — complex/statutory forms into flows | Strevus, PermitNav (in progress) |
| 5 | Workflow & rule builders — nodes vs. forms, validation, versioning | InRule, Flow Builders |
| 6 | Permissions & multi-persona visibility | Acies.ai, PermitNav (in progress) |
| 7 | Onboarding for complex products — time-to-first-value | MeetnGreetMe, ProPortals |
| 8 | Empty, loading, error — states as the product | cross-project |
| 9 | Trustworthy AI output — citations, inspectability | Sprig |
| 10 | Chat is not the product — chat vs. GUI vs. generative UI | PermitNav (in progress), Ten8 |
| 11 | Agent oversight — attention surfaces, human-in-the-loop | Ten8 |
| 12 | Tokens before screens — a design system as AI leverage | Ten8, PermitNav (in progress), TurboCraft |

Patterns 1–8 form the SaaS spine; 9–12 the AI section.

## Positioning line (draft, revisit at launch)

> A field guide to designing complex web apps — for founders, PMs, and AI-era builders shipping products without a design team. Every pattern proven in shipped products.

## Content pipeline

- **Layout:** `content/patterns/<slug>.mdx`, one file per pattern, frontmatter: `title`, `section` (`saas` | `ai`), `status` (`draft` | `review` | `done`), `evidence` (source list). Shared meta in `content/book.md`. Sourcing rules in `content/FACTS.md`.
- **Per-pattern loop:**
  1. Draft skeleton from published case studies; mark every tacit gap `[NEEDS NICK]`.
  2. One batch of 5–8 targeted questions to Nick per pattern; voice-dump answers welcome.
  3. Full draft written in Nick's voice: short sentences, concrete nouns, no corporate verbs.
  4. Nick reviews; revise until approved.
- **Evidence rule:** every "From the field" claim traces to a published case study (vyhouski.com/work) or Nick's verified records. Pre-launch work is described as in progress, never as shipped. Client and customer names appear only where already public. No invented metrics, dates, titles, or tools — ever.
- **Visuals:** redrawn, abstracted diagrams only; no client screenshots unless Nick explicitly clears them. `[VISUAL]` placeholders never block drafting.

## Site

- **Stack:** Next.js (App Router) + MDX, fully static, deployed on Vercel.
- **Page types (3 total):** landing (positioning, grouped pattern index, short author block linking vyhouski.com) · pattern page (six-block anatomy, TOC, prev/next) · about-the-book.
- **Design:** utilitarian craft — fast on 4G, no hero animation, light/dark, accessible. Token-driven from day one; the site practices pattern 12.
- **Visibility:** v1 ships to an **unlisted Vercel preview URL**. Custom domain, public launch, and links from vyhouski.com happen only on Nick's explicit go.
- **Git discipline:** branch per task; nothing pushed to `main` directly.

## Quality bar

A pattern is **done** when: all six blocks are filled · no `[NEEDS NICK]` / `[VERIFY]` markers remain · every field claim traces to a source · Nick has approved the voice · the page renders correctly in Chrome and Safari.

Before any public launch: full sourcing sweep, link check, performance pass (readers are on phones).

Anything unverifiable stays visibly marked rather than smoothed over.

## Open questions (deferred by design)

- Public name + domain (launch-time decision).
- Which real screens/visuals Nick clears for publication.
- Public-launch timing and announcement channels.
