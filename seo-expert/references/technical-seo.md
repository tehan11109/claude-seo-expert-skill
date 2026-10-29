# Technical SEO (sources: Google Search Central, LearningSEO, Moz)

## Crawl & index control
- **robots.txt:** controls crawling only. Never block CSS or JS needed for rendering. Don't use it to deindex pages.
- **Meta robots / X-Robots-Tag:** `noindex` keeps a page out of results. The page must stay crawlable for Google to see the tag.
- **Canonical tags:** `rel="canonical"` on duplicates and parameter variants points to the preferred URL, and self-referencing canonicals belong on originals. Canonicals are a hint, and Google can choose differently. Check in URL Inspection.
- **Redirects:** use 301/308 for permanent moves. Avoid chains and loops. Use 302 only when a move is truly temporary.
- **Status codes:** use 404/410 for gone pages. Avoid "soft 404s" (an error page returning 200). Watch for 5xx errors.
- **XML sitemaps:** include only canonical, indexable URLs that return 200, with accurate `lastmod`. Submit in Search Console and reference in robots.txt.
- **Index coverage:** Search Console → Pages report. "Crawled – currently not indexed" usually means a quality or value problem. "Discovered – not indexed" usually points to crawl priority or site quality.

## Rendering & JavaScript
- Google renders JS, but rendering can be delayed and errors hide content. Prefer SSR, SSG or hybrid rendering (e.g. Next.js) for important content.
- Links must be `<a href="...">`, not JS click handlers.
- Don't load critical content only after user interaction.
- Check with URL Inspection → View crawled page, or compare the rendered HTML against the source.

## Page experience & Core Web Vitals
- **LCP** (loading) ≤ 2.5 s, **INP** (responsiveness) ≤ 200 ms, **CLS** (visual stability) ≤ 0.1, measured at the 75th percentile of real users (CrUX / Search Console CWV report).
- Common fixes:
  - Compress images and use modern formats.
  - Preload the LCP image.
  - Reduce render-blocking JS and CSS.
  - Defer third-party scripts.
  - Set image and video dimensions.
  - Use a CDN and caching.
  - Choose fast hosting.
- Also: HTTPS, mobile-friendly responsive design, and no intrusive interstitials.
- Page experience is a tiebreaker-type signal. Great content on a slow site can still rank, but don't ignore speed. It also affects conversions.

## Mobile-first indexing
Google indexes the mobile version. Make sure mobile has the same content, structured data, metadata and internal links as desktop.

## Site architecture
- Use a logical, shallow hierarchy and descriptive URLs.
- **Pagination:** give each page its own crawlable URL with links between pages. Don't canonicalize page 2+ to page 1.
- **Faceted navigation:** index only facet combinations with real search demand. Use noindex or canonicals and controlled linking for the rest to avoid crawl traps.
- **Crawl budget** matters mainly for large sites (tens of thousands of URLs or more). Remove junk URLs, fix redirect chains and improve server speed. Log file analysis shows what Googlebot actually crawls.

## Structured data
Use JSON-LD that matches the visible content. Validate with the Rich Results Test and the Schema Markup Validator, then monitor the Search Console enhancement reports.

## International / multilingual
- Use separate URLs per language (subfolders like `/si/`, `/ta/`, `/en/` are simplest).
- Add **hreflang** with reciprocal tags, a self-reference and `x-default`. Use language codes `si` (Sinhala), `ta` (Tamil) and `en`, optionally with a region like `en-LK`.
- Don't auto-redirect by IP. Let users switch.
- Translate properly, including titles, meta and URLs where sensible.

## Migrations & redesigns (high-risk)
1. Crawl and export every old URL, along with its traffic and links.
2. Build a 1:1 redirect map to the most relevant new URL.
3. Keep content, titles, internal links and structured data equivalent unless you're improving them deliberately.
4. Test on staging, with noindex on staging and removed at launch.
5. Launch, crawl the old URLs to verify the 301s, submit the new sitemap and use the Change of Address tool for domain moves.
6. Monitor Search Console daily for several weeks. Expect some temporary fluctuation.

## Audit tools
Google Search Console, Bing Webmaster Tools, PageSpeed Insights / Lighthouse, Screaming Frog (free up to 500 URLs), Sitebulb, Ahrefs/Semrush site audit, and the Rich Results Test.
