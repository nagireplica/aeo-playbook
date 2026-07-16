# Platform Testing & Scoring Rubric

Quantitative layer on top of the baseline audit (`baseline-audit.md`). Use the baseline protocol to design queries and interpret strategy; use this rubric when the engagement needs scores that can be tracked over time or compared against competitors.

Adapted from the MIT-licensed [digital-marketing-pro](https://github.com/indranilbanerjee/digital-marketing-pro) plugin (aeo-audit / aeo-geo skills); platform facts as reported there circa mid-2026 — re-verify before citing to clients.

## The six surfaces

Probe each surface separately; they select different sources for the same query:

1. **Google AI Mode** — conversational search tab, default for opted-in users since Google I/O (19 May 2026), ~1B MAUs, Gemini backbone. Supports multi-turn follow-ups; citations evolve across turns, so capture the full thread.
2. **Google AI Overviews** — the summary block on a classic SERP. Triggers on a subset of queries; document which. AI Mode and AI Overviews reportedly disagree on citations for the same query 40–60% of the time (rough estimate — verify against your own probe set). Never roll them into "Google AI".
3. **ChatGPT** — web-search mode on. Responses vary by session; probe 2–3 times per query.
4. **Perplexity** — check both the answer and the cited-sources list.
5. **Gemini** (gemini.google.com) — note any "I don't have enough info" responses.
6. **Microsoft Copilot** — probe in web-grounded mode.

Keep the probe set to 10–25 queries — below 10 the results are anecdotal; above 25, cost and rate limits dominate.

## Per-probe record

| Field | Capture |
|---|---|
| Platform / query / date / model version | For longitudinal comparison |
| Brand mentioned? | Yes / No |
| Mention type | Cited, Recommended, Referenced, Mentioned, Absent, Misrepresented |
| Exact text | Verbatim AI output naming (or omitting) the brand |
| Position | First / middle / last / absent |
| Competitors in same answer | Names, order |
| Source cited | URL if the platform attributes one |
| Accuracy | Yes / Partially / No — fact-check every "brand appears" result |

**Citation accuracy is the most-skipped step.** AI engines confidently hallucinate brand facts; unchecked probes certify wrong information. Fact-check at least the top-cited claim per platform.

## Per-query scoring

| Score | Label | Definition |
|---|---|---|
| 5 | Cited | Brand mentioned with a link to the brand's content as a source |
| 4 | Recommended | Brand explicitly recommended as a top choice |
| 3 | Referenced | Brand named in a relevant context |
| 2 | Mentioned | Brand appears but not usefully |
| 0 | Absent | Brand does not appear |
| −2 | Misrepresented | Brand appears with inaccurate or negative information |

**Score each platform separately — never average across platforms.** A brand can be 9/10-visible on Perplexity (cites everyone) and near-invisible on ChatGPT (selective); the average misleads. Report per-platform scores side by side.

Aggregate per platform: (sum of per-query scores ÷ max possible) × 100. Interpretation bands: 80–100 recognized authority; 60–79 good, citation rate improvable; 40–59 inconsistent; 20–39 weak; 0–19 essentially invisible.

## Competitive benchmarking

Run the identical query set for 2–3 competitors and compare: total visibility score, citation rate (% of queries scoring ≥3), first-mention rate, per-platform strength, and which query categories each brand wins.

## Monitoring cadence

| Scope | Frequency |
|---|---|
| Top ~5 priority queries | Weekly |
| Full query set | Monthly (same queries, same date, logged against the baseline snapshot) |
| Expanded audit with new-query discovery | Quarterly |
| Priority queries on an affected platform | Within 48h of a major model/retrieval update |

Re-audit immediately after: a major AI model release, a large content publish or site restructure, significant schema implementation, a detected competitor visibility change, or an entity correction on Wikipedia/Wikidata.

## Reconciling probes against actuals

Synthetic probes overstate presence — real users phrase queries differently than the test set. Where available, reconcile against measured data:

- **Google Search Console AI Performance Report** (rolled out from 3 June 2026, UK first): actual impressions in AI Overviews + AI Mode for verified properties. No click data by design.
- **GA4 "AI Assistant" channel group** (added May 2026): captures `medium=ai-assistant` referrals from ChatGPT/Gemini/Claude for click-through attribution.

Probe scores show what AI *could* surface; GSC/GA4 show what it *actually* surfaced and what visitors did next.
