# AEO Fundamentals: Platforms, Formats, Tools, Metrics

Background reference for strategy conversations and tool selection. The one-line mental model: SEO helps people find a website; AEO helps AI confidently recommend a business. AEO is an additional optimization layer on top of SEO, not a replacement — the disciplines reinforce each other.

## Platform landscape

Each answer engine retrieves differently, so tactics weight differently per platform:

| Platform | Retrieval basis | What matters most |
|---|---|---|
| ChatGPT | Bing index + licensed content + browsing | Authority, structured content, breadth of mentions |
| Google AI Overviews | Google's search index | Traditional SEO + E-E-A-T + structured data |
| Perplexity | Own crawling + explicit citations | Freshness and credible citable sources |
| Claude | Web search (when enabled) | High-quality, well-structured documentation |
| Gemini | Google ecosystem | Google authority signals |
| Voice assistants (Siri/Alexa) | Knowledge Graph + search | Structured data, business listings |

Practical consequence: freshness work pays off fastest on Perplexity; schema and Business Profile work matter most for Google AI Overviews and voice; broad third-party mentions matter most for ChatGPT.

## Answer-shaped writing

- **Question → answer structure.** Make headings explicit questions ("How much does [X] cost?") rather than clever labels ("Our pricing journey"). LLMs match and quote explicit questions.
- **Answer in the first paragraph**, then elaborate. The direct answer must be complete enough to stand alone when quoted.
- **Structured over prose**: bullets, tables, numbered steps instead of long paragraphs.
- **Specific statistics over vague claims.** "In our analysis of 53 support teams, AI cut first-response time 41%" is retrievable; "AI improves customer service" is not.

## Authority signals (E-E-A-T applied to AEO)

- **Original expertise** is among the strongest differentiators: proprietary customer data, case studies, benchmarks, experiments, surveys. Content nobody else can publish.
- **Identifiable authors**: named author with role, credentials, and a linked profile beats anonymous posts. Add Person/Author schema.
- **Outbound citations** to reputable sources (government, universities, research, industry reports) raise a page's trust.
- **Internal linking as topic clusters**: organize content as a hub with linked spokes (pillar topic → subtopic pages) rather than isolated articles; LLMs read cluster structure as topical authority.

## High-performing content formats

FAQs; comprehensive "ultimate guide" resources (one deep page usually beats many thin ones); comparison pages ("[A] vs [B]" — heavily surfaced by LLMs); how-to content; and definition pages ("What is [term]?"). Use question-research tools (AlsoAsked, AnswerThePublic) to source the questions people actually ask, in their natural phrasing.

## Local businesses

AI assistants pull heavily from business listings: keep Google Business Profile current (hours, services, photos), accumulate reviews, and maintain location pages and local FAQs. For local-intent queries this outweighs most on-site content work.

## Schema checklist

FAQ, Organization, Person, LocalBusiness, Product, Article, HowTo, Review, Event — apply what matches the page type. (Full patterns in `page-anatomy.md`.)

## Tool landscape

Monitoring/AEO-specific: Profound (enterprise citation + competitor tracking), Otterly.ai (entry-level multi-engine monitoring), Peec AI (prompt monitoring + brand mentions), Goodie AI (startup-friendly multi-engine visibility), Scrunch AI (enterprise discoverability). Supporting: Semrush and Ahrefs (authority topics, backlinks, content gaps; both adding AI-visibility features), Screaming Frog (technical crawlability — confirms AI can actually read pages), AlsoAsked / AnswerThePublic (question research for FAQ and content planning).

## Measurement framework

| Metric | Why it matters |
|---|---|
| AI brand mentions | Whether major engines name the brand for relevant prompts |
| AI citation frequency | How often the brand's content is used as a source |
| Share of voice | Visibility relative to competitors across AI answers |
| AI referral traffic | Visits from AI assistant domains |
| Branded search growth | People search the brand name after AI exposure — a lagging indicator of AI recommendations |
| Organic traffic | SEO still matters; watch for cannibalization vs decline |
| Conversion rate | AI-referred users should convert above site average; if not, the pages recommend the wrong buyers |

## Condensed starting workflow

1. Research real user questions (AlsoAsked/AnswerThePublic, sales calls, support tickets).
2. Create comprehensive answer-first content with question headings and structured formatting.
3. Add matching schema.
4. Strengthen authority: original data, case studies, author bios, outbound citations.
5. Build topic clusters via internal linking.
6. Monitor AI visibility (tools above) + manual monthly prompt tests across engines.
7. Refresh content on a schedule; stale statistics quietly kill citations.
