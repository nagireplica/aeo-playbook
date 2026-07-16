# Baseline AI-Visibility Audit Protocol

Produce a dated snapshot of who AI engines currently recommend for the client's target queries. This is step zero of any AEO engagement: it proves progress later, and it usually reorders the plan by revealing which queries are winnable now vs gated by earned media.

## 1. Design the query set (~8 queries)

Cover these archetypes, phrased the way real buyers ask AI:

1. **Broad category** — "best [category] [year]" (hardest to win; reveals the editorial gatekeepers)
2. **Differentiator category** — "best [distinctive-technology/attribute] [category]" (usually most winnable)
3. **Use-case / audience** — "[category] for [specific job/need/situation]"
4. **Niche product feature** — the client's most distinctive feature as a query
5. **Functional phrase** — a plain-language phrase the client could own ("washable X", "X that doesn't Y")
6. **Branded** — "are [brand] [products] good?" (tests whether AI can say anything accurate about the client at all)
7. **Competitor-alternative** — "[incumbent] alternatives that [differentiator]"
8. **B2B/channel** (if relevant) — "[category] brands that sell wholesale / for [business type]"

## 2. Run the queries

Best: run each query in 2–3 actual AI engines (ChatGPT, Perplexity, Google AI Mode and/or AI Overviews — these are distinct surfaces that cite differently; note which one you probed) and record answers verbatim. For a scored, competitor-benchmarked version of this step across all six surfaces, use `platform-scoring.md`. If direct engine access isn't available, approximate with web search — search retrieval is the layer AI engines read before answering, so the domains and brands that dominate retrieval predict what AI will say. Note which method was used; be transparent about the approximation. Dedicated tracking tools (Ahrefs Brand Radar, Otterly.ai, Profound) automate this if the client has access.

Also run one knowledge check: does the AI know the brand exists without retrieval? Young brands typically aren't in training data, which means their AI presence depends entirely on what live retrieval finds.

## 3. Record, per query

- Brands recommended (in order, if ordered)
- Whether the client appears (Y/N, position)
- Which domains/sources are cited or dominate retrieval — this is the key strategic field: it reveals whether the gate is editorial roundups, Reddit threads, review sites, or brand-owned pages
- One-line implication

## 4. Snapshot output template

```
# [Client] AI Visibility Baseline — [date]
## Headline result        (usually: visibility ≈ zero; state it plainly — it's normal and makes progress measurable)
## Query-by-query results (per query: winners / client presence / cited sources / implication)
## Competitor set         (tiered table: incumbents, insurgents, niche specialists — with threat notes)
## Competitive flags      (anything urgent: a competitor using the client's differentiating vocabulary,
                           or a competitor already publishing explicit AEO/for-AI content)
## Monthly re-test protocol (the exact query list, cadence, what to log)
## What this changes about the plan (reordered priorities based on findings)
```

## 5. Interpret

- **Editorial roundups dominate citations** → seeding product to those exact publications outranks any on-site work for that query.
- **Cheap/commodity products dominate a niche** → that niche is the fastest win for a premium, differentiated entrant.
- **A small brand owns a functional phrase** → proof the phrase-ownership play works; pick the client's equivalent phrase.
- **Competitor uses the client's technology vocabulary** → publishing the authoritative explainer page is now time-sensitive.
- **Branded query returns nothing** → a single honest third-party review would become THE cited source for all branded queries; prioritize getting one.

## 6. Milestones to set

- Month 1–2: branded query returns accurate info
- Month 2–4: appears for the weakest-competition niche query
- Month 3–6: named in at least one third-party roundup for the differentiator category
- Month 6+: appears for broad category queries
