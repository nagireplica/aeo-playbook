# Entity Consistency: Cross-Platform Audit & Knowledge Graph Work

AI engines verify who a brand is across independent sources before recommending it. Contradictions (different founding years, conflicting category descriptions, name variants) reduce citation confidence across every surface — and hit personalized surfaces like Google AI Mode hardest, since personalization runs on top of the same entity graph. Practitioner consensus: entity consistency is the single highest-leverage AEO investment, ahead of schema tweaks.

Adapted from the MIT-licensed [digital-marketing-pro](https://github.com/indranilbanerjee/digital-marketing-pro) plugin (aeo-geo skill).

## Audit checklist

For each data point, check every source and mark **Correct / Incorrect / Missing / Outdated**:

| Data point | Sources to check |
|---|---|
| Brand name (exact form) | Google Knowledge Graph, Wikidata, Wikipedia, Crunchbase, LinkedIn, own website schema, industry databases |
| Founding date, founders/CEO, HQ location | same |
| Industry category & product descriptions | same |
| Website URL & social profiles | same |
| Key differentiators / positioning language | same |

## Inconsistency types by severity

| Type | Example | Priority |
|---|---|---|
| Name variation | "Brand Inc" vs "Brand" vs "Brand Corp" — confuses entity resolution | Critical |
| Missing entity | No Wikidata entry at all — reduces AI discovery | Critical |
| Description conflict | "AI platform" on one source, "SaaS tool" on another — category confusion | High |
| Date mismatch | Founded 2019 on Crunchbase, 2020 on LinkedIn | High |
| Leadership outdated | Former CEO listed as current — signals stale data | Medium |
| Address discrepancy | Different cities across sources — hurts local/geo answers | Medium |

Prioritize fixes by source authority weight: Wikipedia/Wikidata > official-site schema > Crunchbase/LinkedIn > directories.

## Google Knowledge Graph

Google builds Knowledge Graph entries from (highest weight first): Wikipedia/Wikidata, schema on the official site, authority databases (Crunchbase, LinkedIn), news mentions, and Google Business Profile for local entities. To optimize:

1. Claim the Knowledge Panel (entity verification via Search Console) and suggest edits for wrong facts.
2. Put Organization schema on the homepage with `sameAs` links to every official profile.
3. Make website, Wikipedia, Wikidata, and authority sources agree — the agreement itself is the signal.
4. Monitor: screenshot the panel on a schedule and compare.

## Wikidata

More permissive than Wikipedia: an entity qualifies with one independent reliable source and a unique identifier in at least one external database. When creating an entry: label, concise description, aliases; properties P31 (instance of), P856 (official website), P571 (inception), P112 (founded by), P159 (headquarters), P452 (industry), plus social identifiers. Every claim needs a reference URL. Never add promotional or subjective claims, and disclose conflict of interest when editing your own company. **Do not edit Wikipedia directly** — earn references instead.

## Common-word brand names

For brands named like ordinary words ("Monday", "Slack" pattern): use the full official name in all structured data, add entity-type qualifiers in descriptions, always co-occur brand + category in content, use Wikidata P1889 (different from) against colliding entities, and schema's `disambiguatingDescription`.

## Monitoring schedule

| Task | Frequency |
|---|---|
| "What is [Brand]?" spot check in AI Mode + AI Overviews (NAP, leadership, description) | Weekly |
| Knowledge Panel screenshot & compare | Weekly |
| Wikidata review for unauthorized edits | Monthly |
| Schema validation (Rich Results Test) | Monthly |
| Full cross-platform consistency scan | Quarterly |
| Crunchbase/LinkedIn/profile updates | Immediately on any real-world change |
| Wikipedia article | Watchlist alerts |
