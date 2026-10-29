# Google Fundamentals (source: Google Search Central)

Primary docs: https://developers.google.com/search/docs. Start with Search Essentials and the SEO Starter Guide.

## How Google Search works (3 stages)
1. **Crawling**: Googlebot discovers URLs, mostly by following links from pages it already knows, and also from sitemaps. It renders pages (including JS) like a browser, so it needs access to the same CSS/JS.
2. **Indexing**: Google analyzes the content, picks a canonical among duplicates, and stores it. Not every crawled page gets indexed.
3. **Serving/ranking**: For each query, Google ranks indexed pages using many signals: relevance, quality, usability, context such as location and language. PageRank (links) is one signal among many.

## Technical requirements (minimum to be eligible for indexing)
- Googlebot can reach the page (not behind a login, not blocked by robots.txt).
- The page returns HTTP 200 (not 4xx/5xx).
- The content is indexable: a supported format, and no spam-policy violations.
- robots.txt blocks **crawling**, not **indexing**. To keep a page out of results, use `noindex` and leave it crawlable.
- Meeting these makes a page *eligible*, but indexing is never guaranteed.

## Key best practices (Search Essentials)
- Write helpful, reliable, people-first content.
- Use the words people actually search for in prominent places: title, main heading, alt text, link text.
- Make links crawlable (`<a href>`), so Google can discover pages.
- Promote the site where the audience already is.
- Follow best practices for images, video, structured data and JavaScript.

## SEO Starter Guide highlights
- Check indexing with a `site:yourdomain.com` search, then use Search Console URL Inspection.
- Changes can take from hours to months to show. Wait a few weeks before judging.
- Use descriptive, human-readable URLs. Group large sites into topic directories.
- Duplicate content isn't a penalty, but it wastes crawling and splits signals. Consolidate with 301 redirects or `rel="canonical"`.
- Content should be easy to read, well organized, original, up to date, and free of distracting ads or interstitials.
- Link to relevant internal and external pages with descriptive anchor text. Mark untrusted or user-generated links with `nofollow`/`ugc`.
- Titles should be unique, clear and concise, and can include the brand. Meta descriptions should be short, unique and accurate (Google often writes its own snippet).
- Images: high quality, near relevant text, with descriptive alt text. Video: on its own page with a descriptive title and description.

## Myths (according to Google)
- Google ignores the keywords meta tag.
- Keyword stuffing violates spam policies.
- Keywords in the domain or URL have minimal effect.
- The TLD matters mainly for country targeting (e.g. `.lk`), and only a little.
- **Content length is not a ranking factor.** There is no magic word count.
- Subdomain vs subfolder is a business decision.
- There's no "duplicate content penalty", but scraped or copied content is a problem.
- Heading order and count don't matter for ranking (they do matter for accessibility).
- **E-E-A-T is not a direct ranking factor.** It's a framework that describes what Google's systems try to reward.

## Helpful, people-first content: self-assessment
**Quality:** Is it original (information, research, analysis)? Is it substantially more valuable than other results? Is the title accurate, not clickbait? Would someone bookmark or share it? Is it free of errors and sloppiness?

**Expertise:** Are sources clear and the author's background visible? Would an expert trust it? Are there factual errors?

**Search-engine-first warning signs:**
- Content made mainly to attract search visits
- Lots of unrelated topics published in the hope some will rank
- Heavy automation
- Summarizing others without adding value
- Chasing trends outside your niche
- Readers needing to search again
- Writing to a word count
- Fake freshness (changing dates without substantive updates)

**E-E-A-T** (Experience, Expertise, Authoritativeness, Trust): trust matters most. It's weighted more heavily for YMYL topics (health, money, safety, civic).

**Who / How / Why:** show who made it (bylines, author pages), how it was made (e.g. how products were tested), and why. The answer to "why" should be "to help people", not "to rank".

**AI content:** allowed if it's people-first. Disclose where readers would expect it. Mass AI output made to rank = scaled content abuse.

## Spam policies (avoid every one of these)
- **Cloaking**: different content for Google than for users
- **Doorway pages**: many similar pages funneling to one destination
- **Expired domain abuse**: buying old domains to host low-value content
- **Hacked content**: injected content or links. Secure the site.
- **Hidden text/links**
- **Keyword stuffing**
- **Link spam**: buying or selling links, excessive link exchanges, automated links, widely distributed footer or widget links, forum-signature links
- **Machine-generated traffic**: automated queries or scraping Google
- **Malicious practices**: malware, back-button hijacking
- **Misleading functionality**: promising tools or services that don't exist
- **Scaled content abuse**: mass low-value pages (AI, scraped or stitched)
- **Scraping**: republishing others' content without added value
- **Site reputation abuse**: hosting third-party content to exploit the host's ranking strength ("parasite SEO")
- **Sneaky redirects**
- **Thin affiliation**: affiliate pages that only copy merchant content
- **User-generated spam**
- **Policy circumvention**
- **Scam and fraud**

Violations lead to algorithmic demotion or manual actions. Check Search Console → Security & Manual Actions.

## Ongoing
- Set up Google Search Console (and Bing Webmaster Tools) on day one.
- Use valid structured data that matches the visible content to become eligible for rich results.
- Follow the Google Search Central blog, the Search Status Dashboard (for update dates) and Search Off the Record.
