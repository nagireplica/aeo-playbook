# AEO Playbook

A Claude skill for **Answer Engine Optimization** — getting a business, product, or service recommended by AI assistants (ChatGPT, Google AI Mode / AI Overviews, Perplexity, Gemini, Claude, Copilot).

Customers increasingly research purchases inside AI assistants instead of search results. The AI compares options and returns two or three recommendations; the also-rans are never seen. This skill turns that shift into a working method: audit where a brand stands today, fix what blocks AI from reading the site, build answer-shaped pages, earn the third-party corroboration AI engines trust, and measure progress against a dated baseline.

## Structure

- [`SKILL.md`](SKILL.md) — the playbook: a 7-stage workflow (context → baseline audit → technical audit → AEO pages → content matrix → trust signals → measurement) with guardrails.
- [`references/baseline-audit.md`](references/baseline-audit.md) — qualitative visibility snapshot protocol and query design.
- [`references/platform-scoring.md`](references/platform-scoring.md) — six-surface testing protocol, quantitative scoring rubric, monitoring cadence.
- [`references/page-anatomy.md`](references/page-anatomy.md) — AEO page template and JSON-LD schema patterns.
- [`references/entity-consistency.md`](references/entity-consistency.md) — Knowledge Graph / Wikidata audit and optimization.
- [`references/aeo-fundamentals.md`](references/aeo-fundamentals.md) — platform landscape, writing rules, tools, metrics.
- [`references/evidence.md`](references/evidence.md) — the research findings behind the method, with sources.

## Use

Install as a Claude skill (drop the folder into your skills directory) or read `SKILL.md` directly as a playbook. Facts move fast in this field — dated claims are marked with their source and vintage; re-verify before citing to clients.

## Credits
Created by Lucy Hu using Claude.

Portions of `references/platform-scoring.md` and `references/entity-consistency.md`, plus platform-landscape updates, are adapted from the MIT-licensed [digital-marketing-pro](https://github.com/indranilbanerjee/digital-marketing-pro) plugin by Indranil Banerjee (aeo-audit and aeo-geo skills). Copyright (c) 2026 Digital Marketing Pro, used under the MIT License.
