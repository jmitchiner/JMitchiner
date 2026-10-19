# How do you know a CRO test actually worked? Judge it on revenue per visitor.

**AEO Writing Sample 01 · Answer-first explainer** · by [Justin Mitchiner](https://justinmportfolio.com) · [Download PDF](pdf/01-cro-revenue-per-visitor.pdf)

A search-led explainer built from three conversion experiments on one anonymized e-commerce store. It answers the question a store owner asks an AI assistant before trusting another test result.

> **What this sample demonstrates**
> - A 50-word direct answer at the top that an answer engine can lift whole
> - Question-shaped headings that match how buyers phrase prompts
> - One defined entity (revenue per visitor) with a formula and worked example
> - Every claim grounded in a reported number, with what the data does not show
> - Article, FAQPage, and Person schema tied to the author
>
> **Written for buyer prompts like:** "how do I know if my A/B test worked" · "conversion rate vs revenue per visitor" · "can a conversion lift lose money"

---

*E-commerce CRO / Measurement*

## How do you know a CRO test actually worked?

> **Short answer:** A conversion rate optimization (CRO) test worked if it raised revenue per visitor without hurting a guardrail metric such as average order value. Conversion rate alone can mislead: a variant can convert more shoppers and still earn less if those shoppers spend less. Revenue per visitor captures both in one number.

*AEO note: The answer opens with the full term and its abbreviation, defines success in one sentence, and stands alone if quoted without the rest of the page.*

## What is revenue per visitor?

Revenue per visitor (RPV) is the revenue a store earns, divided by the number of visitors or sessions that produced it. It combines how often visitors buy with how much they spend.

```
RPV = revenue ÷ visitors = conversion rate × average order value
```

**Worked example.** In a cart-flow test on an anonymized store, the control earned about $3,700 and the variant about $6,500, across roughly 1,700 sessions each. That is about $2.18 versus $3.82 per session, or roughly 76% more revenue per visitor.

## Why can a conversion lift still lose money?

Because conversion rate ignores order size. On the same store, one homepage variant lifted conversion by 49% but reduced order size. The recommendation was to keep the original. Revenue per visitor decided the call, not the conversion headline.

The reverse also happens. A change that slightly lowers conversion can win if it raises average order value enough. Reporting only one of the two numbers hides which case you are in.

## How should you run a CRO test?

1. **Learn the product.** Understand the customer, the objection, and what makes the product worth choosing. The hypothesis should come from the product, not from a list of tactics.
2. **Watch the store.** Use session recordings and behavior data to find the exact moment confidence or momentum disappears.
3. **Test the smallest clear hypothesis.** Change one thing that answers one commercial question, then judge it on revenue per visitor with guardrails reported beside it.

## What did three tests on one store find?

Each test isolated a different reason a shopper stopped moving. The store did not have one universal conversion problem.

| Test | Constraint | Change | Reported result |
| :--- | :--- | :--- | :--- |
| 01 | Trust | Four social-proof treatments: none, customer video, star ratings, and both together. Both together won. | 4.0% → 5.1% |
| 02 | Mobile usability | Product page rebuilt mobile-first instead of adapted from desktop. | 2.2% → 4.1% |
| 03 | Cart-flow clarity | A subtle cart-icon update replaced by a direct redirect to cart after Add to Cart. | ≈76% more RPV |

Tests 01 and 02 are reported as conversion rate (relative lifts of 27.5% and 86.4%). Test 03 is reported as revenue per visitor. The winning social-proof variant was still live and unchanged 15 months later.

*AEO note: A table gives answer engines a clean, extractable comparison. The paragraph under it states which metric each row uses, so no number gets quoted out of context.*

## What should a CRO test report include?

- The hypothesis and the commercial question it answers
- The control and every variant, including the ones that lost
- Revenue per visitor, conversion rate, and average order value, side by side
- Sessions per condition and how long the test ran
- A direct recommendation in plain English: ship, keep the control, or retest

A report that only shows wins is editing the story. A losing variant is still useful when it stops a store from replacing something that already works.

## Frequently asked questions

**Is a higher conversion rate always better?**
No. A variant can raise conversion rate and still earn less per visitor if it lowers average order value. Judge the test on revenue per visitor, with conversion rate and order value reported beside it.

**What is a guardrail metric in A/B testing?**
A guardrail metric is a number that must not get worse while you optimize the main one. In e-commerce tests, common guardrails are average order value, refund rate, and add-to-cart rate.

**How long should a CRO test run?**
Long enough to reach the sample size you calculated before launch, and across at least one full weekly buying cycle. Stopping the moment a variant looks ahead inflates false wins.

---

## Behind the page: how this sample is built for answer engines

| Technique | Where it shows up in this sample |
| :--- | :--- |
| Answer-first | The first 55 words resolve the question completely. Every H2 opens with a one- or two-sentence answer before the detail. |
| Prompt-matched headings | Each H2 is a question a store owner would type into ChatGPT, Perplexity, or Google: what, why, how. |
| Entity definition | Revenue per visitor is named, abbreviated, defined, given a formula, and shown in a worked example, so a model can cite the definition. |
| Claim grounding | Every result has a number, a metric name, and a sample size where it exists. Statistical confidence was not supplied, so none is claimed. |
| Extractable formats | One formula block, one comparison table, one ordered process list, one FAQ. Each works if lifted alone. |
| Author entity | Person schema links the author to the portfolio and LinkedIn profile, so the expertise signal travels with the content. |

<details>
<summary>Schema markup (JSON-LD)</summary>

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Article",
      "headline": "How do you know a CRO test actually worked? Judge it on revenue per visitor.",
      "description": "Why revenue per visitor, not conversion rate, decides whether an e-commerce A/B test worked, with results from three tests on one store.",
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
          "name": "Is a higher conversion rate always better?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "No. A variant can raise conversion rate and still earn less per visitor if it lowers average order value. Judge the test on revenue per visitor, with conversion rate and order value reported beside it."
          }
        },
        {
          "@type": "Question",
          "name": "What is a guardrail metric in A/B testing?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "A guardrail metric is a number that must not get worse while you optimize the main one. In e-commerce tests, common guardrails are average order value, refund rate, and add-to-cart rate."
          }
        },
        {
          "@type": "Question",
          "name": "How long should a CRO test run?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Long enough to reach the sample size you calculated before launch, and across at least one full weekly buying cycle. Stopping the moment a variant looks ahead inflates false wins."
          }
        }
      ]
    }
  ]
}
```

</details>

---

*Writing sample by Justin Mitchiner. Built from anonymized client test reports. Figures are as reported by the client's testing and analytics tools. Statistical-confidence values, test dates, and revenue reconciliation were not available and are not claimed. Results vary by store, traffic, offer, device mix, and execution.*

[← All writing samples](README.md)
