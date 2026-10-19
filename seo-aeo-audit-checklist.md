# SEO & AEO (Answer Engine Optimization) Audit Checklist

*This checklist outlines my methodology for auditing a B2B SaaS website's content architecture. It ensures the site is optimized not just for traditional Google search (SEO), but for AI-driven search engines and LLMs (AEO).*

---

## Phase 1: Technical SEO Foundation

Before optimizing for AI, the traditional search foundation must be flawless.

| Check | Item | Description |
| :--- | :--- | :--- |
| [ ] | **Indexability** | Ensure `robots.txt` and `sitemap.xml` are correctly configured and no critical pages are blocked. |
| [ ] | **Site Speed & Core Web Vitals** | Verify LCP, INP, and CLS meet Google's "good" thresholds in field data (CrUX / Search Console), not just lab scores. (INP replaced FID as a Core Web Vital in March 2024.) |
| [ ] | **Mobile Responsiveness** | Confirm the site is fully optimized for mobile-first indexing. |
| [ ] | **URL Structure** | Ensure URLs are clean, descriptive, and use hyphens (e.g., `/b2b-content-strategy`). |
| [ ] | **Canonical Tags** | Check that canonical tags are properly implemented to prevent duplicate content issues. |
| [ ] | **JavaScript Rendering** | Confirm primary copy, headings, links, and metadata exist in the initial HTML response. Many AI crawlers do not execute JavaScript, so client-side-only content can be invisible to them. |
| [ ] | **AI Crawler Access** | Review `robots.txt` rules for AI crawlers (e.g., GPTBot, OAI-SearchBot, ClaudeBot, PerplexityBot, Google-Extended) and make a deliberate allow/block decision for each. |

## Phase 2: On-Page SEO & Content Quality

Evaluating the existing content against current search intent and quality standards.

| Check | Item | Description |
| :--- | :--- | :--- |
| [ ] | **Keyword Intent Alignment** | Does the content actually answer the user's search intent (Informational, Navigational, Transactional)? |
| [ ] | **Title Tags & Meta Descriptions** | Are they optimized for CTR, under character limits, and containing primary keywords? |
| [ ] | **Header Hierarchy (H1, H2, H3)** | Is the content logically structured? Is there only one H1 per page? |
| [ ] | **Content Depth & Freshness** | Is the content comprehensive compared to top-ranking competitors? Is it up-to-date? |
| [ ] | **Internal Linking Architecture** | Are topic clusters properly linked? Are orphan pages eliminated? |

## Phase 3: Answer Engine Optimization (AEO)

Optimizing content to be retrieved and cited by AI answer surfaces (Google AI Overviews and AI Mode, ChatGPT search, Perplexity, Gemini, Claude).

| Check | Item | Description |
| :--- | :--- | :--- |
| [ ] | **Direct Answer Formatting** | Are core questions answered directly and concisely (under 50 words) immediately following the heading? |
| [ ] | **Structured Data (Schema Markup)** | Are Organization, Person, Article, Product/Service, and BreadcrumbList schema implemented and valid? (Google now limits FAQ and HowTo rich results, but structured data still clarifies entities for machines.) |
| [ ] | **Information Density** | Does the content provide unique data, statistics, or expert quotes that LLMs prioritize over generic text? |
| [ ] | **Entity Optimization** | Are industry-specific entities clearly defined and linked to authoritative sources? |
| [ ] | **AI Citation Tracking** | Is there a baseline for how often the brand is mentioned or cited for priority queries across AI answer engines, re-checked on a set cadence? |
| [ ] | **Formatting for Skimmability** | Are lists, tables, and bullet points used effectively? (LLMs parse structured formats easier than walls of text). |

## Phase 4: Conversion & UX

Traffic is useless if it doesn't convert.

| Check | Item | Description |
| :--- | :--- | :--- |
| [ ] | **CTA Placement** | Are primary and secondary CTAs visible without being intrusive? |
| [ ] | **Message Match** | Does the landing page copy match the intent of the search query or ad that drove the traffic? |
| [ ] | **Readability** | Is the font size, contrast, and spacing optimized for easy reading? |
