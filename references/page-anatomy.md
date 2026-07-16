# AEO Page Anatomy

The template for a product or landing page optimized for AI answer engines. Adapt sections to context (product page, service page, use-case page, B2B page) — the ordering logic stays constant: answer first, facts dense, structure machine-readable.

## Section order

1. **Title + meta description** — clear, not clever. State product, category, and differentiator: "[Name]: [what it is] | [key differentiator] | [Brand]". Meta description packs the buying facts: what, who for, price, sizes/variants, return policy.
2. **Hero / answer header** — H1 that names the thing and its category. Immediately below: price, availability, variant range, return window, rating (if genuinely earned).
3. **Quotable answer block** — an H2 like "What is [X]?" followed by 2–4 sentences that fully answer what it is, how it differs, and who it's for. Write this paragraph as if it will be quoted verbatim by an AI, because it will be. Bold the load-bearing phrases.
4. **Use-case grid** — one card per audience/problem ("for [specific job]", "for [specific condition]", "for [context]"). Each card: who, why this product fits their exact situation, one concrete detail. These cards are what let AI match niche queries.
5. **Specification list** — label/value bullets: construction, materials, care, variants, price, returns, anything measurable. Numbers over adjectives.
6. **Comparison table** — "[X] vs [the incumbent alternative]": feature rows, honest cells (concede where the incumbent wins, e.g. price), one-line bottom-line under the table telling each buyer type which to choose. Balanced comparisons earn AI trust; one-sided ones get discounted.
7. **Social proof** — real quotes with attribution. Never fabricate. If review count is low, use quotes but hold off on AggregateRating schema until volume justifies it.
8. **FAQ** — 8–12 questions phrased the way people actually ask AI (durability, sizing, care, comparisons to siblings/competitors, shipping, wholesale). Answers: 2–3 self-contained sentences each. Mirror exactly in FAQPage schema.
9. **B2B block** (when relevant) — wholesale/partner value proposition and a contact path, so distributor-type queries have a destination.
10. **Freshness marker** — visible "last updated" date; refresh at least every 6 months.

## JSON-LD schema patterns

Include three blocks (plus Organization sitewide). Check what the platform already auto-emits (e.g., Shopify emits Product) and extend rather than duplicate — conflicting duplicate schemas are worse than none.

**Product** — name, brand, description (mirror the quotable answer block), image, url, sku, material, color, category, offers (price, priceCurrency, availability, priceValidUntil, hasMerchantReturnPolicy), additionalProperty for distinctive attributes (manufacturing method, care, size range). Only include aggregateRating/review with real, sufficient volume.

**FAQPage** — mainEntity array mirroring the on-page FAQ word-for-word. This is the most directly liftable schema for answer engines.

**BreadcrumbList** — home → category → page. Teaches AI the site's category structure.

Facts in schema must match facts in visible text exactly — mismatches read as manipulation.

## Writing rules

- Every claim traceable to the client or their live site; flag inferred details (return windows, materials, certifications) for verification before publishing. Wrong facts on an AEO page become wrong facts in AI answers about the brand.
- Concrete numbers wherever possible (weights, counts, times, percentages) — fact density measurably raises citation rates.
- No superlatives without substantiation; regulated claims (health, sustainability) need evidence or get cut.
- Headlines literal, not punny. "Machine-washable slip-on shoe" beats "Freshness, reinvented."
- Write FAQ answers as standalone units — each must make sense quoted alone, without the surrounding page.

## Placement

Build on the client's existing canonical domain, never a standalone microsite: domain-level trust signals (reviews, press, backlinks) accrue to one domain, and a fresh single-product domain reads as thin/spammy while splitting the truth about the product across two sources. Upgrade the existing product URL rather than creating a duplicate page; spin use-case sections out to their own URLs on the same domain as the content matrix grows.
