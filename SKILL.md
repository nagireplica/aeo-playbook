---
name: aeo-playbook
description: Answer Engine Optimization (AEO) — make a business, product, or service get recommended by AI assistants like ChatGPT, Gemini, Perplexity, Claude, and Google AI Overviews. Use this skill whenever the user asks how to get recommended, cited, mentioned, or found by AI; wants an AEO/GEO/LLM-SEO strategy; asks why AI doesn't recommend their product; wants to build or optimize product pages, landing pages, or content for AI visibility; wants an AI-visibility audit or baseline; or mentions "answer engine optimization," "generative engine optimization," "AI search," or "showing up in ChatGPT." Also trigger when a user asks how AI shopping recommendations work commercially, or wants a website revision plan focused on AI discoverability — even if they never use the term AEO.
---

# AEO Playbook: Getting Recommended by AI Answer Engines

## Why this matters (read first)

Customers increasingly research purchases inside AI assistants instead of browsing search results. The AI reads the web, compares options, and returns two or three recommendations; the customer never sees the also-rans. This changes the funnel: by the time a visitor reaches a website, an AI has often already prequalified them. Businesses that get recommended receive fewer but far more purchase-ready visitors (industry measurements put LLM-referred e-commerce conversion at roughly 5.5% vs 3.7% for organic search).

The AI is effectively the business's first salesperson. AEO is the practice of giving that salesperson everything it needs: readable facts, precise matches for niche queries, and third-party corroboration.

Traditional SEO instincts actively mislead here — the overlap between top Google results and AI-cited sources has collapsed to under 20%, and pages with zero search volume can be valuable because AI matches hyper-specific queries to hyper-specific pages.

## Workflow

Users rarely need every stage. Identify which stage the request maps to, confirm scope, then execute. Recommended order for a full engagement: 0 → 1 → 2 → 3 → 4 → 5 → 6.

### Stage 0 — Establish context (always do this)

Before advising, learn: what the business sells, price point, audience(s), business model (DTC, B2B, marketplace, local service), current site platform, and what "winning" means (sales, leads, partners, awareness). If the user names a real company, fetch their actual site and product data — never invent specs, prices, review counts, or policies. Anything not verifiable (return windows, materials, certifications) gets flagged for the user to confirm before publication, because AEO pages teach AI engines facts about the brand; publishing wrong facts spreads misinformation with the brand's name on it.

### Stage 1 — Baseline visibility audit (do this before building anything)

You cannot prove progress without a before-picture. Read `references/baseline-audit.md` and produce a dated snapshot: which brands AI currently recommends for the target queries, whether the client appears, who gets cited, and what that implies for sequencing. The baseline routinely reorders the plan — e.g., discovering that editorial roundups gate the biggest queries, or that a competitor already owns the client's differentiating vocabulary.

### Stage 2 — Site and technical audit

Check, in order of leverage:

1. **One canonical domain.** Multiple live sites (old platform + new, www vs apex serving different content) split authority and feed AI conflicting facts. Consolidate with 301 redirects before anything else.
2. **AI crawler access.** robots.txt must allow GPTBot, ClaudeBot, PerplexityBot, Google-Extended. Blocked crawlers = invisible brand.
3. **Crawlability of content.** Fetch key pages the way a crawler does. JS-rendered pages that return empty shells are invisible regardless of quality. Server-rendered text is non-negotiable for pages that must be read.
4. **Structured data.** Product, Organization, FAQPage, BreadcrumbList schema. Schema is how an AI knows price, availability, and what the thing is. Check for existing platform-generated schema first (Shopify and others auto-emit Product schema) — extend it, never duplicate it; two conflicting Product schemas is worse than one.
5. **Placeholder/unfinished content** (default banners, lorem ipsum) — signals an untrustworthy source.
6. **Site architecture.** Does a page exist for each thing the business wants to be recommended for (technology story, fit/sizing, wholesale, FAQ)? AI cannot cite pages that don't exist.

### Stage 3 — Build AEO pages

Read `references/page-anatomy.md` for the full template and schema patterns. Core principles:

- **Lead with the answer.** The first paragraph must directly, quotably answer "what is this and who is it for." AI engines lift answer-shaped paragraphs.
- **Hyperspecific beats general.** Build pages for every meaningful combination of product × audience × problem × geography, even with zero Google search volume. They need to be crawlable, not ranked.
- **Fact density.** Concrete numbers, named materials, measured claims, and cited statistics raise citation odds substantially (studies show up to ~40% visibility lift). Vague marketing copy gets skipped.
- **Machine-shaped structure.** Headings phrased as explicit questions ("How much does X cost?", never "Our pricing journey"), bullets, spec lists, comparison tables, FAQ blocks mirrored in FAQPage schema.
- **Authority signals.** Named authors with credentials (Person schema) instead of anonymous posts; outbound citations to reputable sources; original data (case studies, benchmarks, surveys) that nobody else can publish — the strongest differentiator.
- **Honest comparisons.** "X vs Y" content including competitors outperforms pure self-promotion — AI trusts balanced sources. Never fabricate competitor weaknesses.
- **Visible freshness.** Most AI citations for commercial queries go to pages updated within the last 12 months. Add "last updated" dates and a refresh cadence (≤6 months for key pages).

### Stage 4 — Content matrix

Replace top-of-funnel blogging with bottom-of-funnel, purchase-intent pages:

- **Use-case pages**: one per audience/problem ("[product category] for [specific job/need/context]").
- **Comparison pages**: client vs each named competitor; construction-type vs construction-type.
- **Curated "best of" category pages**: the single biggest e-commerce AEO opportunity, because "best X for Y" is the dominant AI query shape. Include competitors honestly.
- **B2B intent pages** if relevant: wholesale, partnership, bulk-order pages so distributor-type queries have a destination.
- **Definition and how-to pages** for the category's key terms — heavily surfaced formats.

Source the questions from reality: question-research tools (AlsoAsked, AnswerThePublic), sales calls, and support tickets reveal how buyers actually phrase things. Organize pages as topic clusters (pillar page + internally linked subtopics) rather than isolated posts — cluster structure reads as topical authority. Cadence over volume: 2–3 solid pages per week, each refreshed on schedule, beats a launch burst that goes stale.

For local businesses, weight listings over content: Google Business Profile freshness, review volume, location pages, and hours/services data are what AI assistants pull for local-intent queries.

### Stage 5 — Trust signals (often more important than on-site work)

AI systems exhibit a measured bias toward earned media — third-party sources — over anything a brand says about itself. Reddit has been the single most-cited domain by LLMs. For a low-authority brand, perfect on-site pages may sit uncited for months; third-party corroboration is what unlocks them. Prioritize:

1. **Editorial roundups.** Identify which publications' "best X" articles get cited for the target queries (the baseline audit reveals this) and pitch/seed product for testing. This is usually the gate to the biggest queries.
2. **Reddit and community forums.** Genuine, disclosed participation in the subreddits where the category is discussed. Never astroturf — AI surfaces the callouts too.
3. **Review corpus.** Automate post-purchase review collection; push reviews to third-party surfaces (Google, Trustpilot, category-specific sites), not just the brand's own site. Caution: don't publish AggregateRating schema on a handful of reviews — it reads as thin or manipulative. Build volume first.
4. **Video reviews.** YouTube is heavily cited and dominates younger-demographic discovery. Seed products to relevant reviewers.
5. **Entity consistency.** Identical company description across site schema, LinkedIn, business registries, and (once notable) Wikidata. AI verifies who you are across sources before recommending.

### Stage 6 — Measurement

Attribution is inherently leaky (research happens in the AI, purchase happens days later on-site), so instrument proactively:

- Add "AI assistant (ChatGPT/Gemini/Perplexity)" to post-purchase "how did you hear about us" surveys.
- Segment analytics referrals from AI domains (chatgpt.com, perplexity.ai, gemini.google.com).
- Re-run the baseline query set monthly (same queries, same date, log results against the snapshot).
- Consider AI-mention monitoring tools (entry tier ~$29/mo) once budget allows.
- Judge lead quality, not just traffic volume — expect traffic down, conversion up.

Set realistic milestones: branded queries answerable within 1–2 months; niche category visibility in 2–4; broad "best of" inclusion typically 6+ and gated by earned media.

## Guardrails

- **No invented facts.** Every spec, price, policy, or claim on an AEO page must come from the user or their live site, or be flagged as needing verification. Sustainability and health-adjacent claims need substantiation before publishing.
- **AEO complements, never replaces, the rest of marketing.** Position it alongside paid, social, email, and conversion work — it is an evolving channel with hard attribution, not a bet-the-company strategy.
- **Match effort to authority.** For young/low-authority brands, weight Stage 5 earlier and heavier; for established brands, Stages 2–4 unlock faster.
- **Strategy questions deserve strategy answers.** If the user asks "how does this connect to sales," explain the funnel shift plainly before prescribing tactics.

## References

- `references/baseline-audit.md` — visibility snapshot protocol, query design, output template. Read when auditing current AI visibility or setting up measurement.
- `references/page-anatomy.md` — full AEO page section order, JSON-LD schema patterns, worked generic example. Read before building or reviewing any page.
- `references/evidence.md` — the research findings behind the method, with numbers. Read when the user wants justification, sources, or a strategy document.
- `references/aeo-fundamentals.md` — platform-by-platform landscape (ChatGPT vs Perplexity vs AI Overviews vs voice), answer-shaped writing rules, E-E-A-T/authority signals, content formats, tool directory, and the measurement metrics table. Read for strategy explanations, tool selection, or platform-specific questions.
