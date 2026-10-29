# Troubleshooting: Not Ranking, Traffic Drops, Core Updates (sources: LearningSEO, Google)

## "Why doesn't my page rank?": work through in order
1. **Crawlable?** HTTP status, robots.txt, login walls, JS-only links. (Search Console URL Inspection)
2. **Indexable & indexed?** `noindex` in meta or headers, the canonical pointing elsewhere, removal requests. Is it in "Pages → Not indexed"?
3. **Relevant enough?** Does it match the SERP's intent (3 Cs)? Does it cover what the top results cover?
4. **More helpful and trustworthy than the top results?** Depth, originality, first-hand experience, authorship, accuracy.
5. **Good page experience?** CWV, mobile, HTTPS, intrusive pop-ups.
6. **Internally linked?** Reachable from navigation or relevant pages, and in the sitemap? Not orphaned?
7. **Backlink gap?** Compare referring domains and their quality with the pages that rank.
8. **Good links disavowed by mistake?**
9. **Manual action or security issue?** Check Search Console.
10. **Search appearance?** If it ranks but gets few clicks, improve the title and meta and add eligible structured data.
11. **Cannibalization?** Another URL on the site competing for the same query.
12. **Patience?** New pages and sites can take weeks to months, especially in competitive niches.

## Traffic drop diagnosis
1. **Is it real?** Check tracking changes (GA4 tags, consent banners), seasonality (compare year over year with Google Trends) and reporting mistakes.
2. **Search Console vs. analytics:** if clicks dropped in Search Console, it's search-related. If only GA dropped, it's probably tracking.
3. **When exactly?** Compare the date against the Google Search Status Dashboard (core, spam and other updates) and the site's own deploy log (migrations, redesigns, robots/noindex mistakes, CMS updates).
4. **Where?** Segment by page, query, device, country and search type. Is it sitewide (technical problem or site-quality reassessment) or limited to some pages or sections (intent shift, competitors, cannibalization)?
5. **Impressions or CTR?** If impressions dropped, you lost rankings. If impressions are stable but clicks fell, it's a SERP change: AI Overviews, more ads, new features, or a worse snippet.
6. **Check the SERPs** for the lost queries. Who replaced you, and why? Did the intent change? (Forums, video and big brands often appear after updates.)

## Core update recovery
- Core updates reassess overall content quality and relevance. There's no single "fix" and no penalty to remove.
- Map the drop onto update dates, then identify the affected pages and queries (segment in Looker Studio or a sheet).
- Compare affected pages honestly against Google's helpful-content questions and E-E-A-T: thin, outdated or unoriginal content, weak authorship, an ad-heavy experience, or content outside the site's expertise.
- Improve the site as a whole: upgrade or merge weak content, prune pages with no value, add real expertise and experience, and fix UX and technical issues. Don't make cosmetic changes such as editing dates or doing word-count padding.
- Recovery often comes at a later core update, which can mean months. Keep improving and keep notes.

## Manual actions
Read the exact reason in Search Console, fix every instance (for unnatural links, remove or disavow them), document what you did and submit a reconsideration request.

## Hacked site / spam injection
Check Security Issues and use `site:` searches for strange pages (e.g. pharma or casino spam in Japanese). Clean up the site, patch it (update CMS and plugins, change credentials), then request a review.
