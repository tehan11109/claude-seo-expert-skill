# E-commerce, Local & Multilingual SEO (sources: Shopify, Yoast, Google, LearningSEO)

## E-commerce (Shopify, WooCommerce, etc.)
**Architecture**
- Homepage → categories/collections → (subcategories) → products. Keep it shallow.
- Link key collections from the main navigation and use breadcrumbs.
- Category/collection pages usually target the head commercial terms ("men's running shoes"). Product pages target specific model and variant searches.

**Product pages**
- Write unique descriptions. Copied manufacturer text creates thin, duplicate pages.
- Include specs, sizing, use cases, real photos and video, shipping and returns info, and FAQs.
- Reviews add fresh, unique content and trust. Use Product schema with `offers`, `aggregateRating` and `review` where the data is genuine.
- **Out of stock:** temporary → keep the page live (200) and show the availability status. Discontinued → 301 to the closest replacement or category, or 404/410 if nothing fits.

**Category pages**
- Add a short, useful intro or buying guide (not a block of keyword text), clear filters and internal links to subcategories.

**Duplicates & facets**
- Products reachable via several collection paths: Shopify canonicalizes `/collections/x/products/y` to `/products/y`, so internal links should point to the canonical.
- Variants: one URL with variant parameters, canonicalized.
- Faceted filters: index only combinations with demand (e.g. "red dresses"). Noindex, canonicalize or block the rest.

**Platform notes**
- Shopify:
  - Edit title and meta on every product and collection.
  - Watch for app bloat that slows the site.
  - Shopify generates the sitemap and robots.txt automatically, and robots.txt can be customized via `robots.txt.liquid`.
- WordPress/WooCommerce:
  - Use an SEO plugin (Yoast, Rank Math) for titles, sitemaps and schema.
  - Noindex thin tag and attachment pages.
  - Use good hosting and caching.

**Merchant Center:** free listings in Google Shopping. Keep the feed's price and availability matching the site.

**Links for stores:** gift guides, niche bloggers and reviewers, supplier and manufacturer "where to buy" pages, local press and data-driven PR.

## Local SEO (shops, clinics, restaurants, service businesses)
- **Google Business Profile:**
  - Choose the correct primary category and complete every field: hours, services/products, photos, attributes.
  - Post updates and answer Q&A.
  - Get genuine reviews and reply to all of them. Never buy reviews.
- **NAP consistency:** the same business Name, Address and Phone on the site, GBP and directories. Sri Lankan examples: lankapropertyweb, ikman for some categories, the Yellow Pages Sri Lanka, chambers and industry associations.
- **Location pages:** one strong page per real location, with unique content (directions, local team, local photos and reviews). Avoid near-duplicate city-swap pages.
- **LocalBusiness schema** with address, geo, hours and phone.
- **Local links & mentions:** local news, events, sponsorships, partners.
- Ranking factors Google names: **relevance, distance, prominence**.

## Multilingual / Sri Lanka specifics
- Many users search in English, Sinhala (සිංහල), Tamil (தமிழ்) and transliterated Singlish ("hoda phone eka"). Research each language separately. Volumes differ a lot, and Sinhala-script content often faces less competition.
- Use separate language URLs with hreflang (`si-LK`, `ta-LK`, `en-LK`, plus `x-default`). Use real translation and localization, not raw machine output.
- Use Unicode Sinhala/Tamil text (not images of text or legacy fonts) so it can be indexed.
- `.lk` vs `.com`: `.lk` is a geotargeting signal. A `.com` targeting Sri Lanka works fine with local content, local links and hreflang.
- Local trust signals: an LKR price display, local phone number and address, and local payment options.
