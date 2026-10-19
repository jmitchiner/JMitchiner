# Editing a strong post into one AI answers can quote

**AEO Writing Sample 06 · Editorial AEO pass** · by [Justin Mitchiner](https://justinmportfolio.com) · [Download PDF](pdf/06-editorial-aeo-pass.pdf)

A second editorial pass on a roughly 2,400-word guide I ghostwrote for Alinea Business, published under the founder's byline as "AI Search Visibility: Why AI Doesn't Recommend Your Business." The post already does a lot right. This pass targets what stops an answer engine from quoting it.

> **What this sample demonstrates**
> - Reviewing my own published work as critically as a client's
> - Rewriting claim headings as the questions they answer
> - Giving each question one answer on the page instead of two
> - Adding a summary table answer engines can lift whole
> - Pairing the edits with the technical fixes that make them count
>
> **Written for buyer prompts like:** "how do I get my business recommended by ChatGPT" · "what is AI search visibility" · "how do I measure AI search visibility"

---

*Editorial pass / Published guide on AI search visibility*

## What does this editorial pass change?

> **Short answer:** It keeps the post's argument, sources, and voice, and changes how the answers are found. Claim headings become questions. Three sections that repeat FAQ answers are merged, so each question has one answer on the page. A summary table, schema, and a fix to the blog's canonical tag make the answers easy for an engine to lift and possible to index.

## What the post already does well

- **A definition up front.** The key section opens with one sentence defining AI search visibility as how accurately and often a business appears in AI-generated answers.
- **Primary sources.** Claims about crawling, structured data, and Search Console reporting link to Google's and OpenAI's own documentation.
- **Direct FAQ answers.** All five FAQ answers open with the answer before the context.
- **A clear sequence.** Six ordered steps: technical access, positioning, profiles, content, third-party proof, measurement.

## Edit 1: Make every heading the question it answers

Only the FAQ uses question headings. The 12 body sections use declarative claims, which read well but do not match how buyers phrase prompts.

| Published H2 | Edited H2 | Note |
| :--- | :--- | :--- |
| What AI search visibility actually means | What is AI search visibility? | |
| AI cannot clearly describe a business that describes itself vaguely | Why doesn't AI recommend my business? | |
| Make sure AI search systems can access the website | Can AI search tools crawl my website? | |
| Keep your business information consistent across the web | Why does consistent business information matter for AI search? | |
| Use structured data as clarification, not as a shortcut | Do I need special schema for AI search? | Merge with FAQ 3 |
| Create content that proves what you know | What content gets cited in AI answers? | |
| Strengthen the evidence beyond your own website | Do third-party mentions affect AI recommendations? | |
| Reviews help establish category relevance and trust | Do reviews affect AI search visibility? | |
| Traditional SEO and AI visibility support each other | Is AI SEO different from traditional SEO? | Merge with FAQ 2 |
| Traditional rank tracking only tells part of the story | How do I measure AI search visibility? | Merge with FAQ 5 |
| Test the questions customers actually ask | How do I test what AI says about my business? | |
| Fix the clearest visibility gaps first | Where should I start? | |

## Edit 2: Give each question one answer

Three body sections answer the same questions as FAQs 2, 3, and 5. Two answers to one question split the signal and invite a model to quote the weaker one. The full answer stays in the body section. The FAQ keeps a two-sentence version that links to it.

## Edit 3: Open every section with the answer

Each section gets a first sentence that resolves its heading on its own. For example:

> **Can AI search tools crawl my website?**
> They can if robots.txt allows the crawlers that feed AI search, such as Googlebot, Bingbot, OAI-SearchBot, and PerplexityBot, and your key pages are indexable with their main content in the HTML. Check those three things before any content work.

## Edit 4: Add a summary table

The six-step sequence becomes a table near the top. It is the single most quotable block in the post.

| Step | Fix | What to check |
| :--- | :--- | :--- |
| 1 | Technical access | Crawlers allowed, pages indexable, canonicals correct, main content in the HTML |
| 2 | Positioning | One plain sentence on what the business does, for whom, and where |
| 3 | Profiles | Name, category, and description match across every profile and directory |
| 4 | Content | Case studies, process breakdowns, and findings that prove expertise |
| 5 | Third-party proof | Earned mentions and detailed reviews that name the category |
| 6 | Measurement | A fixed prompt set, retested monthly, plus AI referral traffic in analytics |

## Edit 5: Clean up and mark up

- **Remove the drafting leftover.** "The original email makes an important point" is rewritten as a direct claim.
- **Fix the canonical.** The post's canonical points to a URL that returns 404 ([Sample 05](05-ai-search-readiness-audit.md), finding 1). None of these edits matter until the page can be indexed.
- **Add schema.** BlogPosting linked to the founder and organization already defined on the main site, plus FAQPage for the remaining FAQs.

<details>
<summary>Schema markup (JSON-LD)</summary>

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "BlogPosting",
      "headline": "AI Search Visibility: Why AI Doesn't Recommend Your Business",
      "datePublished": "2026-07-31",
      "mainEntityOfPage": "https://blog.alineabusiness.com/post/ai-search-visibility",
      "author": { "@id": "https://alineabusiness.com/#founder" },
      "publisher": { "@id": "https://alineabusiness.com/#organization" }
    },
    {
      "@type": "FAQPage",
      "mainEntity": [
        {
          "@type": "Question",
          "name": "How do I get my business recommended by ChatGPT?",
          "acceptedAnswer": { "@type": "Answer", "text": "[answer text exactly as published on the page]" }
        },
        {
          "@type": "Question",
          "name": "Is AI SEO different from traditional SEO?",
          "acceptedAnswer": { "@type": "Answer", "text": "[answer text exactly as published on the page]" }
        },
        {
          "@type": "Question",
          "name": "Do I need special schema for AI search?",
          "acceptedAnswer": { "@type": "Answer", "text": "[answer text exactly as published on the page]" }
        },
        {
          "@type": "Question",
          "name": "Does a high Google ranking guarantee AI visibility?",
          "acceptedAnswer": { "@type": "Answer", "text": "[answer text exactly as published on the page]" }
        },
        {
          "@type": "Question",
          "name": "How can I measure whether AI systems mention my business?",
          "acceptedAnswer": { "@type": "Answer", "text": "[answer text exactly as published on the page]" }
        }
      ]
    }
  ]
}
```

</details>

> **Schema rule:** FAQPage answer text must match what is visible on the page. The placeholders are filled from the published copy at build time.

---

*Editorial pass by Justin Mitchiner on a post he ghostwrote for Alinea Business, published under founder Jeff Welsh's byline. Justin writes all posts on the Alinea blog and builds and manages the site. Checked October 17, 2026.*

[← All writing samples](README.md)
