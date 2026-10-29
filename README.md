# SEO Expert: a Claude Skill

An end-to-end SEO practitioner skill for [Claude](https://claude.ai) and Claude Code. It turns Claude into an SEO consultant that follows Google's official guidance first, treats tool metrics as estimates, and frames advice as testable experiments rather than "secret hacks".

The skill is built from research across the most trusted free SEO resources, based on a resource list shared by Sri Lankan SEO consultant **Sathmina Dissanayake**:

- [Google Search Central](https://developers.google.com/search): Search Essentials, SEO Starter Guide, spam policies, helpful content, AI features
- [LearningSEO.io](https://learningseo.io/) by Aleyda Solis
- [Ahrefs Blog & Academy](https://ahrefs.com/blog/)
- [Moz](https://moz.com/blog)
- [Backlinko](https://backlinko.com/)
- [Search Engine Journal](https://www.searchenginejournal.com/) and [Search Engine Roundtable](https://www.seroundtable.com/)
- [Surfer Blog](https://surferseo.com/blog/)
- [Yoast SEO Blog](https://yoast.com/seo-blog/) and [Shopify Blog](https://www.shopify.com/blog)

All content is summarized and paraphrased. Follow the links above for the original material.

## What it covers

| Area | Reference file |
|---|---|
| How Google works, technical requirements, spam policies, myths | `references/google-fundamentals.md` |
| Keyword research, search intent (3 Cs), clustering, cannibalization | `references/keyword-research.md` |
| On-page SEO, content quality, E-E-A-T, semantic SEO, topic clusters | `references/on-page-and-content.md` |
| Crawling, indexing, canonicals, Core Web Vitals, JS, migrations, hreflang | `references/technical-seo.md` |
| Link building, digital PR, outreach, disavow | `references/link-building.md` |
| E-commerce (Shopify/WooCommerce), local SEO, multilingual (Sinhala/Tamil/English) | `references/ecommerce-local-international.md` |
| Why a page doesn't rank, traffic drops, core update recovery | `references/troubleshooting.md` |
| AI Overviews, AI Mode, ChatGPT/Perplexity visibility | `references/ai-search.md` |
| Learning roadmap and trusted resources | `references/learning-roadmap.md` |

It also includes ready-made output formats for SEO reviews, content briefs, keyword plans and strategy roadmaps.

## Install

**Claude Code** (personal skill):

```bash
git clone https://github.com/tehan11109/claude-seo-expert-skill.git
cp -r claude-seo-expert-skill/seo-expert ~/.claude/skills/
```

Or copy `seo-expert/` into a project's `.claude/skills/` folder to share it with a team.

**Claude.ai:** zip the `seo-expert` folder and upload it under Settings → Capabilities → Skills.

## Usage

Just ask SEO questions, and the skill triggers automatically. Examples:

- "Audit the SEO of https://example.lk"
- "Why isn't my blog post ranking on Google?"
- "Do keyword research for a Colombo-based café"
- "Write an SEO-friendly article on choosing a laptop in Sri Lanka"
- "Our traffic dropped 40% last week, help me find out why"

In Claude Code you can also invoke it directly with `/seo-expert`.

## Philosophy

> Theory shows you the road, but real SEO is learned in the field.

Read the guides, then build your own test site, publish, measure, and learn from the failures.

## License

MIT
