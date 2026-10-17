# Book-Application-Product-Design-Patterns

A public web book of product-design patterns for complex web applications. Working title: Application Product Design Patterns. The public name is chosen at launch.

Status: design spec only. The repo has no site code or chapter content yet.

## What it covers

- Audience: founders, PMs and builders shipping complex web apps without a design team, whether they brief a designer or prompt an AI coding tool.
- Scope: the recurring surfaces and decisions of B2B SaaS web apps, plus a section on AI product patterns. The spec lists 12 candidate patterns, 8 of them SaaS and 4 AI.
- v1 target: any 8 of the 12 patterns live at an unlisted URL, at least 2 from the AI section.
- Each chapter uses the same six blocks: the situation, forces, the pattern, from the field, anti-patterns, build it with AI.

## Planned stack

Per the spec: Next.js (App Router) with MDX, fully static, deployed on Vercel. Chapters live in `content/patterns/<slug>.mdx`. None of this exists in the repo yet.

## Files

- `docs/superpowers/specs/2026-08-02-book-design.md`: the design spec (goals, audience, pattern anatomy, v1 scope, content pipeline, site plan, quality bar, open questions).
