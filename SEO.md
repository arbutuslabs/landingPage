# Arbutus Labs - SEO Documentation

This document outlines the SEO strategy and technical implementations performed for the Arbutus Labs website (arbutuslabs.ca) to improve search engine rankings, local visibility in Vancouver and Western Canada, and overall site authority.

## 1. Technical SEO Foundations

### Keyword-Rich Title Tag
- **Content:** "Arbutus Labs | AI Automation for Small Businesses in Vancouver, BC"
- **Why:** Leads with the brand, then the primary service keyword ("AI Automation"), target market ("Small Businesses"), and geographic focus ("Vancouver, BC"). This is the single most important on-page ranking signal.

### Optimized H1
- **Content:** "Your time is worth too much to spend on admin"
- **Why:** The H1 is user-facing and conversion-focused while the supporting paragraph immediately below contains the keyword-dense copy: "AI systems for small businesses in trades, real estate, and law." This two-layer approach satisfies both user experience and search engines.

### Schema.org Structured Data
- **Type:** `ProfessionalService`
- **Properties Included:**
  - Name, Logo, URL, and Email.
  - **Founder:** Tyson Chernen, with `alumniOf` linking to Queen's University.
  - **Address:** Vancouver, BC, Canada.
  - **Area Served:** 500 km radius from Vancouver (covers Western Canada).
  - **Knows About:** AI Automation, Business Process Automation, Custom AI Systems, Knowledge Systems, Small Business AI, Workflow Automation.
  - **Price Range:** `$$` (signals mid-range professional service).
- **Benefit:** Helps Google generate Rich Results and Knowledge Graph entries. The `ProfessionalService` type is the best fit for a consultancy that builds and maintains AI systems.

### Metadata & Open Graph
- **Meta Description:** "Arbutus Labs builds and maintains custom AI systems for trades, real estate, and law firms in Vancouver. Automate admin, scheduling, and follow-ups — so you stay focused on clients." (Under 155 characters for optimal SERP display.)
- **Open Graph:** Title, description, type, URL, image, and site_name tags ensure the site looks polished when shared on LinkedIn, Facebook, or Slack.
- **Twitter Card:** `summary_large_image` card type with matching title, description, and image for Twitter/X shares.
- **Theme Color:** `#2D3B28` (brand sage green) — controls the browser tab color on mobile.

### Canonical URL
- **Value:** `https://arbutuslabs.ca/`
- **Why:** Prevents duplicate content issues if the site is accessible via multiple URLs (www vs non-www, trailing slash, GitHub Pages URL, etc.).

---

## 2. Content & Image Optimization

### Descriptive Alt Text
- **Strategy:** Every image uses context-rich alt tags that include the brand name and service keywords.
- **Examples:**
  - Nav logo: "Arbutus Labs — AI automation for small businesses in Vancouver, BC"
  - Portrait: "Tyson Chernen, founder of Arbutus Labs — AI automation consultant in Vancouver"
  - Client logos: "[Client Name] — AI automation client of Arbutus Labs"
- **Why:** Alt text is a ranking signal for image search and provides context to search engines about the page's topic. Including "AI automation" and "Vancouver" reinforces local + service relevance.

### Lazy Loading
- **Implementation:** All client logo images use `loading="lazy"`.
- **Why:** Defers off-screen image loading to improve initial page load speed, which directly affects Core Web Vitals (LCP) — a confirmed Google ranking factor.

### Internal Linking
- **CTA Buttons:** Both "Start with a free conversation" buttons link to `#contact`, creating internal anchor links that help search bots understand page structure.
- **Nav Email:** Direct `mailto:` link preserved for users who prefer email.

---

## 3. Local SEO Signals

### Geographic Keywords
- **In Title:** "Vancouver, BC"
- **In Meta Description:** "in Vancouver"
- **In Schema:** Full address (Vancouver, BC, Canada) + 500 km service radius.
- **In Footer:** "Vancouver, BC" visible on every page load.
- **In Contact Section:** "Vancouver, BC" with "Serving Western Canada" subtext.
- **Why:** Consistent NAP (Name, Address, Phone-equivalent) signals across structured data, visible content, and metadata tell Google this is a legitimate local business.

### Service-Area Keywords
- **Industries mentioned:** Trades, real estate, law firms, small businesses.
- **Placement:** Hero paragraph, "Who We Work With" section, Schema `knowsAbout` array.
- **Why:** Long-tail keywords like "AI automation for law firms Vancouver" are lower competition and higher intent than generic "AI automation."

---

## 4. Performance & Accessibility

### Selection Color
- **Implementation:** `::selection { background: var(--accent); color: var(--bg); }` — branded text selection highlight.
- **Why:** Small detail that signals a polished, intentionally designed site. Does not directly affect SEO but improves perceived quality (which reduces bounce rate).

### Smooth Scroll & Anchor Offset
- **Implementation:** `scroll-behavior: smooth` on `html`, `:target { scroll-margin-top: 40px }` for anchored sections.
- **Why:** Prevents content from being hidden behind fixed elements when navigating via anchor links. Better UX = lower bounce rate = indirect SEO benefit.

### Font Preconnect
- **Implementation:** `<link rel="preconnect">` for Google Fonts domains.
- **Why:** Reduces font load latency by establishing early connections, improving First Contentful Paint (FCP).

---

## 5. Recommended Next Steps

1. **Google Business Profile:** Create a GBP listing for "Arbutus Labs" at your Vancouver address. This is the #1 lever for local search visibility.
2. **Sitemap & robots.txt:** Add `sitemap.xml` and `robots.txt` to the root for better crawl efficiency (especially once you add more pages).
3. **Blog / Case Studies:** Adding a `/blog` or `/case-studies` page with write-ups on client projects (e.g., "How we automated scheduling for Urbanek Law") would target long-tail keywords and build topical authority.
4. **Backlinks:** Get listed on local Vancouver business directories and ask clients to link back to arbutuslabs.ca from their sites.
5. **Google Search Console:** Submit the site and monitor indexing, impressions, and click-through rates.

---
*Last Updated: May 2026*
