# An AI-search readiness audit of a site I built, misses included

**AEO Writing Sample 05 · Technical AEO audit** · by [Justin Mitchiner](https://justinmportfolio.com) · [Download PDF](pdf/05-ai-search-readiness-audit.pdf)

A technical and content audit of alineabusiness.com and its blog subdomain. It runs the checks that decide whether Google's AI Overviews, ChatGPT search, and Perplexity can find, trust, and cite a business. Checked October 17, 2026.

> **What this sample demonstrates**
> - Checking the crawl, canonical, and index signals AI search depends on
> - Reading structured data as one connected description of the business, not a checklist
> - Ranking fixes by their effect on being cited, not by how many there are
> - Reporting what works next to what is broken, including my own build
> - Turning findings into fixes a developer or marketer can ship this week
>
> **Written for buyer prompts like:** "why doesn't ChatGPT mention my business" · "is my site ready for AI search" · "how do I rebrand without losing search visibility"

---

*alineabusiness.com / Checked October 17, 2026*

## Is alineabusiness.com ready for AI search?

> **Short answer:** The main site is. Every route serves prerendered HTML with its own canonical, and the core pages carry connected schema for the business, its founder, its FAQ, and its offers. The blog is not. Every post checked points its canonical at a URL that returns 404 with noindex. The pages most likely to be quoted in AI answers are the least likely to be indexed. And the agency's former brand is still live as a separate site, which splits the business into two entities.

| Main site | Blog | Fixes |
| :--- | :--- | :--- |
| **Strong**<br>7 routes checked | **At risk**<br>4 posts checked, all affected | **10**<br>1 critical, 3 high, 3 medium, 3 low |

## What is working

| Signal | What is in place | Why it matters for AI search |
| :--- | :--- | :--- |
| ✅ Server-rendered content | Headings and full body copy are in the raw HTML on every route checked, before any JavaScript runs. | Not every AI crawler runs JavaScript. Text in the first HTML response can be read by all of them. |
| ✅ Per-route metadata | Each route has its own title, meta description, and a canonical that points to itself. | Tells engines which URL to index, rank, and cite. |
| ✅ Organization + founder graph | Organization and founder Person are linked by `@id`, with founding date and a one-line description. | Gives engines one consistent statement of who the business is and who runs it. |
| ✅ FAQPage schema | `/faq` marks up 19 questions across six topics. | Question-and-answer pairs map directly to how buyers phrase prompts. |
| ✅ Service + Offer schema | Each free audit page is described as a Service with an Offer. | Makes every offer a distinct thing an engine can name and describe. |
| ✅ Crawl access | robots.txt allows all crawlers. The sitemap is generated at build time with lastmod dates. | No AI search crawler is blocked, and fresh pages are announced. |

## What needs fixing, in priority order

| # | Priority | Finding | Evidence | Fix |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **Critical** | Blog canonicals point to a dead page. | All four posts checked on blog.alineabusiness.com declare their canonical as `alineabusiness.com/post/…`. That URL returns a 404 with `noindex`. Search engines are being told the preferred version of each post does not exist. | Point each canonical at the post's own URL, or serve the blog at that path on the main domain. This is usually one domain setting in the blog platform. Then request reindexing in Search Console. |
| 2 | High | Blog robots.txt and sitemap are empty. | Both files return a 200 status with no content, so crawlers get no list of posts to find. | Publish both files and submit the blog sitemap in Search Console. |
| 3 | High | Blog posts have no structured data. | No Article or BlogPosting markup, and no FAQPage markup, even though posts include FAQ sections (five in the AI search post, six in the Meta scaling post). | Add BlogPosting with the author linked to the founder `@id`, plus FAQPage for each post's FAQ section. |
| 4 | High | The previous brand is still live as a separate business. | thinkimpakt.com, the agency's former brand, still serves a full site as "Impakt Results." It does not redirect and never mentions Alinea. Alinea's schema has no `alternateName` or link to the old brand. Engines see two unrelated agencies, and the older domain likely holds most of the history and backlinks. | If the old site is not being kept on purpose, 301-redirect each page to its closest Alinea equivalent. Add `alternateName` for the old brand to the Organization schema, and update profiles and directories that still list Impakt. |
| 5 | Medium | The case study headline figure does not match its PDF. | The page says 8.72X ROAS. The PDF says 8.70x, which matches the source math ($211,392.24 ÷ $24,302.61 = 8.70). The page also has no structured data. | Use 8.70x everywhere. Conflicting figures cost trust with readers and with models. Add Article markup for each case study. |
| 6 | Medium | Thin entity links. | Organization `sameAs` lists only the community subdomain. The founder Person has no `sameAs` at all. | Add the brand's and the founder's official LinkedIn, YouTube, and other profiles so engines can connect the business to its other appearances on the web. |
| 7 | Medium | The SEO report page lags the blog. | The SEO Visibility Report page has a five-question FAQ with no FAQPage markup. It never mentions AI search, while the blog argues AI visibility matters. | Add FAQPage markup now. Add AI-search checks to the page only when the report actually includes them. |
| 8 | Low | The Why Alinea page has no structured data. | This is the page the founder schema already points to as his URL. | Add AboutPage markup that references the Organization and founder. |
| 9 | Low | The calculator does not show its math. | The Revenue Leak Calculator names its five levers but not its formulas or where its benchmarks come from. | Publish the method and benchmark sources. A tool that shows its working can be cited. A black box cannot. |
| 10 | Low | A drafting leftover is live on the blog. | The AI search post includes the line "The original email makes an important point". | Rewrite the sentence. Leftover drafting notes undercut a post about credibility. |

> **Why #1 comes first:** Google's AI Overviews draw on Google's index, and ChatGPT search and Perplexity draw on search indexes too. A post that is not indexed cannot be cited, however well it is written. Fixing one setting protects every post already published.

> **On FAQ markup:** Since 2023, Google shows FAQ rich results for only a narrow set of sites. FAQPage markup is recommended here because it makes question-and-answer pairs easier for machines to parse, not for a search-results feature.

## How the audit was run

1. Fetched the raw HTML, before JavaScript, for seven main-site routes and four blog posts.
2. Recorded each page's title, meta description, canonical, robots meta, H1 and H2 structure, and every JSON-LD block.
3. Requested every canonical target and logged its status code and robots directive.
4. Fetched robots.txt, sitemap.xml, and llms.txt on both hosts. The site has no llms.txt. That file is an optional proposal that no major engine has said it uses, so it is not counted as a finding.
5. Read the two most recent posts for structure, sources, and editorial issues.

**Not covered here:** actual index status in Search Console, live AI citation results, Core Web Vitals, and backlinks. Those need account access or a monthly prompt log (see [Sample 03](03-prompt-space-map.md)).

---

*Audit by Justin Mitchiner of a site he built and manages, and a blog he writes. Findings reflect the live site and blog on October 17, 2026, checked from outside without account access. thinkimpakt.com is the agency's previous brand site. The brand, founder, and published figures named here are public.*

[← All writing samples](README.md)
