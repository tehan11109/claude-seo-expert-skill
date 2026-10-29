---
name: seo-expert
description: End-to-end SEO practitioner playbook built from Google Search Central, LearningSEO.io (Aleyda Solis), Ahrefs, Moz, Backlinko, Surfer, Yoast, Shopify and Search Engine Journal, filtered through a field-tested "experience over theory" mindset. Use this skill whenever the user wants to rank a website, plan SEO strategy, do keyword research, optimize a page or blog post, fix indexing or crawling problems, diagnose a traffic or rankings drop, recover from a Google core update, build backlinks, do e-commerce/Shopify/WordPress SEO, local SEO (Google Business Profile), multilingual SEO (e.g. Sinhala/Tamil/English sites), or show up in AI Overviews/ChatGPT answers. Also use it when the user asks "how do I learn SEO", "why isn't my page ranking", "write an SEO-friendly article", "SEO plan for my client", or shares a URL and asks how to get more Google traffic — even if they don't say the word "SEO".
---

# SEO Expert

A practitioner's SEO skill. It combines what Google officially documents with the best-known industry playbooks, and keeps one mindset throughout: **search engines are a black box, tools sell themselves, and real SEO is learned by testing on real sites.**

## Core principles (apply to every task)

1. **Google's own docs are the source of truth.** When industry advice and Google Search Central disagree, follow Google and say so. Google knows how its system works better than any third party. See `references/google-fundamentals.md`.
2. **Treat tool metrics as estimates, not facts.** Ahrefs KD, Moz DA, Semrush AS and Surfer scores are third-party models, and the blogs that publish them are partly marketing for those tools. Use them for direction, and verify against the live SERP and Search Console data.
3. **Nobody knows "secret ranking hacks".** Don't promise rankings or invent ranking factors. Separate what's *confirmed* (Google docs), *widely observed* (industry studies), and *your hypothesis to test*. Label which is which.
4. **People first, search engines second.** Every recommendation should make the page more useful to the human searcher. If a tactic only exists to manipulate rankings, it's probably a spam-policy risk.
5. **Experiment and measure.** Recommend changes as testable hypotheses: what to change, what metric should move (Search Console clicks/impressions/position, GA conversions), and how long to wait (usually weeks; core-update recovery can take months).
6. **SEO changes fast, especially with AI search.** For anything time-sensitive (algorithm updates, new SERP features, AI Overviews behaviour), check recent news before answering. Search Engine Roundtable, Search Engine Journal and the Google Search Central blog are good sources. Don't rely on memory alone.
7. **Don't overwhelm.** Prioritize. Give the 3–5 highest-impact actions first, ordered by impact ÷ effort, then the rest.

## Workflow: figure out the job, then load the right reference

| User wants… | Read |
|---|---|
| Understand how Google works, rules, spam policies, myths | `references/google-fundamentals.md` |
| Keyword research, topic ideas, search intent, keyword mapping | `references/keyword-research.md` |
| Write or optimize a page/article, titles, meta, headings, topic clusters | `references/on-page-and-content.md` |
| Indexing, crawling, canonicals, redirects, speed, JS, sitemaps, migrations | `references/technical-seo.md` |
| Backlinks, digital PR, outreach, disavow | `references/link-building.md` |
| Shopify/WooCommerce stores, local businesses, multilingual sites | `references/ecommerce-local-international.md` |
| "My page doesn't rank", traffic drop, core update, manual action | `references/troubleshooting.md` |
| AI Overviews, AI Mode, ChatGPT/Perplexity visibility | `references/ai-search.md` |
| "How do I learn SEO?", learning roadmap, which resources to follow | `references/learning-roadmap.md` |

Most real requests touch more than one area. A new-site plan, for example, needs keyword research, on-page and technical. Read every reference that applies.

## Gather context first

Before giving advice, establish (or ask briefly for whatever's missing):
- **The site:** URL, CMS (WordPress, Shopify, Wix, custom/Next.js…), age, approximate size.
- **The goal:** traffic, leads, sales, local calls, brand visibility. SEO goals must tie to business goals.
- **Market:** country/city and language(s). Sri Lanka, for instance, may need Sinhala, Tamil and English versions plus local intent.
- **Data available:** Google Search Console, GA4, any paid tool. Search Console is the most trustworthy data source, so ask for it when diagnosing.
- **Constraints:** budget, dev access, content team.

If the user shares a URL and you can fetch it, inspect the actual page (title, meta, headings, canonical, robots meta, structured data, internal links, content) instead of speaking generically.

## Output formats

**SEO audit / site review**: use this structure:
```
# SEO Review: <site>
## Summary (3–5 sentences: biggest problems + biggest opportunities)
## Priority actions (table: # | Issue | Why it matters | Fix | Impact | Effort)
## Technical findings
## On-page & content findings
## Authority / links findings
## What to measure (metrics + where + when to re-check)
```

**SEO content brief** (for a writer or for you to write the article):
```
# Content brief: <primary keyword>
- Search intent + 3Cs (type / format / angle) from the live SERP
- Primary keyword, secondary/related terms, entities to cover
- Suggested title tag (≤ ~60 chars) and meta description (≤ ~155 chars)
- H1 and outline (H2/H3), each section answering one sub-question
- Unique value to add (first-hand experience, data, examples, local angle)
- Internal links (to/from), external sources to cite
- Schema type if relevant; FAQ from real "People also ask" questions
```

**Keyword plan**: a table: Keyword | Intent | Parent topic/cluster | Volume or traffic potential (say if estimated) | Difficulty (estimated) | Business potential 0–3 | Target URL (new or existing).

**Strategy / roadmap**: phases (Foundation → Content → Authority → Iterate), each with concrete tasks, owner, and success metric.

## Writing SEO content yourself

When asked to write an article or page:
1. Determine intent from the SERP (or reason carefully about it if you can't search).
2. Answer the main question early, then expand. Use short paragraphs and descriptive H2s that each make sense on their own. This helps both skimmers and AI answer engines.
3. Add something the top results don't have: experience, specific examples, local context, original data, or a clearer explanation. Don't write to a word count. Length is not a ranking factor.
4. Use the primary keyword naturally in the title, H1, intro, and at least one subheading, plus related terms and entities. Never stuff keywords.
5. Provide the title tag, meta description, URL slug, suggested internal links and alt text alongside the content.
6. If content is AI-assisted, recommend human review for accuracy and a real author byline. Google allows AI content but penalizes scaled, low-value content made mainly to rank.

## The reality check (always worth including in strategy advice)

Reading guides builds a foundation, but most of the craft comes from practice. Encourage the user to:
- Build their own small test site on a cheap domain and try ranking pages.
- Watch what happens during algorithm updates and keep notes.
- Expect strategies to fail sometimes, and treat failures as data.
- Not to try to learn everything at once, because that leads to burnout. Pick a starting point and go deep.
