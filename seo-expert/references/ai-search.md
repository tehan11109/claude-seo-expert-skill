# AI Search: AI Overviews, AI Mode, ChatGPT, Perplexity (sources: Google, LearningSEO)

This area changes monthly. Check recent news before giving confident specifics.

## What Google officially says
- No special "AI SEO" is required. To appear as a supporting link in AI Overviews or AI Mode, a page must be indexed and eligible to show with a snippet. Normal SEO best practices apply.
- Google says you need no special files, markup or schema for AI features (`llms.txt` is not used by Google Search).
- Helpful practices:
  - Allow crawling (robots.txt, CDN or firewall).
  - Use internal linking.
  - Provide a good page experience.
  - Put important content in text.
  - Make structured data match the visible content.
  - Keep Merchant Center and Business Profile up to date.
- AI features use "query fan-out", running many related searches. A wider range of pages can be cited, including ones that don't rank top 3 classically.
- **Measurement:** AI feature traffic is included in Search Console's Performance report (Web). Use GA4 for engagement and conversions.
- **Controls:** `nosnippet`, `data-nosnippet`, `max-snippet` and `noindex` limit what's shown. The `Google-Extended` token controls use for Gemini training and grounding, not Search.

## Practical optimization (industry consensus, not guarantees)
- **Chunk content:** sections that stand alone, each starting with a direct answer to a clear question. AI systems retrieve passages, not whole pages.
- **Cover the fan-out:** address the follow-up and related questions a user would ask next.
- **Be quotable:** specific facts, numbers, definitions, comparisons and original data, with clear attribution.
- **Entity clarity:** consistent brand name and descriptions everywhere (site, social profiles, Wikipedia/Wikidata if eligible, directories). Use Organization schema with `sameAs`.
- **Brand mentions across the web:** LLMs learn from and retrieve popular sources such as Reddit, YouTube, review sites, news and "best X" listicles. Being mentioned there drives AI visibility.
- **Other engines:**
  - ChatGPT search relies largely on Bing's index, so set up Bing Webmaster Tools and IndexNow.
  - Perplexity has its own crawler (PerplexityBot).
  - Check that robots.txt doesn't block crawlers you want (OAI-SearchBot, PerplexityBot, Bingbot).
- **Track:** manually test prompts for target topics, use AI visibility trackers (several SEO tools offer them) and segment GA4 referral traffic from chatgpt.com, perplexity.ai, gemini, copilot and similar sites.

## The "great decoupling" / zero-click reality
Impressions can rise while clicks fall because answers are shown in the SERP. Re-evaluate KPIs:
- Visibility and share of voice
- Branded search growth
- Conversions per click
- AI citations

Don't rely only on raw sessions.
