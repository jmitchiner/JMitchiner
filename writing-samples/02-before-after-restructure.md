# Rewriting a case study so answer engines can cite it

**AEO Writing Sample 02 · Before / after restructure** · by [Justin Mitchiner](https://justinmportfolio.com) · [Download PDF](pdf/02-before-after-restructure.pdf)

The same motorsports e-commerce story, written twice. First, the original case-study copy, built to persuade a reader who is already on the page. Then the same facts restructured so ChatGPT, Perplexity, and Google's AI Overviews can find, trust, and quote them.

> **What this sample demonstrates**
> - Turning slogan headlines into question-shaped headings
> - Defining an industry term (fitment data) in the first sentence
> - Replacing vague scale words with specific, sourced figures
> - Stating what a result does and does not prove, so a model quotes it accurately
> - Keeping the brand's voice while changing the structure
>
> **Written for buyer prompts like:** "what is fitment data" · "why do online parts stores lose sales" · "does fixing product data improve ROAS"

---

*Motorsports parts e-commerce / Anonymized client*

## Four changes, side by side

The facts do not change between versions. What changes is the order they arrive in, the questions the headings answer, and how much a reader, or a model, has to infer.

### Change 1

| Before · original | After · answer-first |
| :--- | :--- |
| **Parts buyers do not browse. They search.**<br><br>A rider replacing a specific part usually knows the make, model, and year. If the store cannot confirm fitment quickly, the sale moves to a competitor that can. | **Why do online parts stores lose high-intent buyers?**<br><br>Parts stores lose high-intent buyers when they cannot confirm fit quickly. Shoppers search by make, model, and year. If a search does not return a part they trust will fit, they buy from a store that can confirm it. |

**Why:** The original headline is a strong line for a human reader, but no one types it into an AI assistant. The question heading matches the prompt, and the first sentence answers it.

### Change 2

| Before · original | After · answer-first |
| :--- | :--- |
| **7,541 fitment records. Made live and searchable.**<br><br>A single bolt kit can fit multiple machines across several manufacturers and model years. The automated import missed many of those cross-brand relationships. | **What is fitment data, and what happens when it is missing?**<br><br>Fitment data is the record of which vehicles a part fits, usually stored as make, model, and year combinations. When an import misses cross-brand matches, a part that fits never appears in the search. On this store, 7,541 cross-brand fitment records were reviewed, approved, and made searchable. |

**Why:** "Fitment" is never defined in the original, because the reader already knows it. A model needs the definition to understand and repeat the claim, and a newcomer searching the term gets an answer.

### Change 3

| Before · original | After · answer-first |
| :--- | :--- |
| **Same event. Less spend. More than double the attributed sales.**<br><br>The second year produced more than twice the Meta-attributed purchase value on slightly less media spend. | **Can you improve ROAS without raising ad spend?**<br><br>Yes. This retailer ran the same national-event campaign two years running. Meta-attributed purchase value rose from $103,228 on $6,000 of spend to $209,981 on $5,844, about 2.6% less. Reported ROAS went from 17.2x to about 35.9x. |

**Why:** "Slightly less" and "more than twice" are true but hard to cite. Exact figures, with the attribution source named, give a model something concrete to quote and a reader something to check.

### Change 4

| Before · original | After · answer-first |
| :--- | :--- |
| **The event did not change. The system did.**<br><br>Better audience signals, cleaner fitment coverage, stronger creative learning, and more deliberate follow-up. | **What drove the improvement?**<br><br>Four changes landed between the two campaigns: fitment coverage, audience signals built from the first year's purchases, creative learning, and intent-based follow-up. The data shows the combined result. It does not isolate how much came from each change. |

**Why:** The original line implies fitment alone did it. The rewrite names every factor and says what the data cannot separate. That protects the claim when an engine summarizes it, and it is more honest.

---

## The restructured page: how the finished version reads, top to bottom

> **Short answer:** Online parts stores lose high-intent buyers when they cannot confirm fit. Fixing fitment data, the make, model, and year records that match parts to vehicles, makes more searches end on a product page. For one motorsports retailer, fixing that data and the follow-up around it helped double Meta-attributed sales from the same event on 2.6% less spend.

| Section | Heading | Job |
| :--- | :--- | :--- |
| 1 | Why do online parts stores lose high-intent buyers? | Names the problem in the buyer's words |
| 2 | What is fitment data, and what happens when it is missing? | Defines the entity, gives the 7,541-record fix |
| 3 | Can you improve ROAS without raising ad spend? | The year-over-year result with exact figures |
| 4 | What drove the improvement? | All four factors, and what the data cannot isolate |
| 5 | What does Meta-attributed purchase value prove? | Verified versus not shown, stated plainly |
| 6 | Frequently asked questions | Short, quotable answers with FAQ schema |

### Section 5: What does Meta-attributed purchase value prove?

It proves what Meta's attribution credits to the campaign: $6,000.00 producing $103,228.38 in 2025 and $5,844.24 producing $209,981.42 in 2026. It does not show order counts, average order value, margins, refunds, or profit after fulfillment. Attribution is evidence, not audited revenue.

### Frequently asked questions

**What is fitment data?**
Fitment data is the record of which vehicles a part fits, usually stored as make, model, and year combinations. It decides whether a shopper's vehicle search returns the right product.

**Why do parts stores lose high-intent shoppers?**
Because parts buyers search by vehicle. If the store cannot confirm fit quickly, the shopper buys from a competitor that can. Missing fitment hides products that would have fit.

---

## Behind the rewrite

| Technique | Where it shows up in this sample |
| :--- | :--- |
| Answer-first | A 70-word short answer covers the problem, the fix, and the result, and each section opens with its answer. |
| Entity disambiguation | Fitment data is defined once, in plain terms, the first time it appears. The vehicle is described as make, model, and year, which is how buyers search. |
| Claim grounding | Vague scale words are replaced with exact figures, the attribution source is named, and the 2.6% spend change is stated precisely rather than rounded. |
| Causal honesty | The rewrite does not credit the result to any single change, so an AI summary cannot overstate it. |
| Voice kept | Short declarative sentences and the line "attribution is evidence" carry over from the original. |

<details>
<summary>Schema markup (JSON-LD)</summary>

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Article",
      "headline": "Why online parts stores lose high-intent buyers, and how fitment data fixes it",
      "description": "How fixing 7,541 fitment records and the follow-up around them helped one motorsports retailer double Meta-attributed sales from the same event.",
      "author": {
        "@type": "Person",
        "name": "Justin Mitchiner",
        "jobTitle": "Content Marketing Manager & SEO/AEO Strategist",
        "url": "https://justinmportfolio.com",
        "sameAs": ["https://www.linkedin.com/in/justinmitchiner"]
      }
    },
    {
      "@type": "FAQPage",
      "mainEntity": [
        {
          "@type": "Question",
          "name": "What is fitment data?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Fitment data is the record of which vehicles a part fits, usually stored as make, model, and year combinations. It decides whether a shopper's vehicle search returns the right product."
          }
        },
        {
          "@type": "Question",
          "name": "Why do parts stores lose high-intent shoppers?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Because parts buyers search by vehicle. If the store cannot confirm fit quickly, the shopper buys from a competitor that can. Missing fitment hides products that would have fit."
          }
        }
      ]
    }
  ]
}
```

</details>

---

*Writing sample by Justin Mitchiner. The "before" copy is from the author's own portfolio case study. Client identity is anonymized. Purchase value and ROAS are Meta-reported attribution measures, not audited cash revenue, fulfilled orders, or profit. Figures here are rounded to one decimal place for ROAS and to the nearest dollar in the short answer.*

[← All writing samples](README.md)
