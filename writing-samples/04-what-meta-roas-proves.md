# What does Meta ROAS actually prove? Attribution is evidence, not mythology.

**AEO Writing Sample 04 · Definitional reference page** · by [Justin Mitchiner](https://justinmportfolio.com) · [Download PDF](pdf/04-what-meta-roas-proves.pdf)

A reference page that defines reported ROAS, shows how to calculate it, and draws a clear line between what an ad dashboard verifies and what it cannot. Built from a six-month anonymized e-commerce account, $24,302.61 in spend and $211,392.24 in Meta-attributed sales.

> **What this sample demonstrates**
> - A definitional page built to be the source an AI assistant cites
> - A verified-versus-not-shown table, the most quotable format on the page
> - Worked calculations a reader can check line by line
> - Correcting a common misread (dashboard "net profit" is not profit)
> - FAQ answers written to stand alone when extracted
>
> **Written for buyer prompts like:** "is my Meta ROAS real" · "what is a good ROAS" · "why does Meta show different sales than Shopify"

---

*Paid media / Measurement*

## What does Meta ROAS actually prove?

> **Short answer:** Meta-reported ROAS (return on ad spend) shows how much purchase value Meta's attribution model credits to your ads for each dollar spent. It is real evidence of ad performance, but it is not audited revenue or profit. It leaves out product cost, fulfillment, refunds, and overhead, and it counts sales the way Meta attributes them, not the way your bank does.

## How is reported ROAS calculated?

```
Reported ROAS = Meta-attributed purchase value ÷ ad spend
```

**Worked example.** Over six months, one e-commerce account spent $24,302.61 and Meta attributed $211,392.24 in sales to it.

| Attributed sales | Ad spend | Reported ROAS |
| :--- | :--- | :--- |
| **$211,392**<br>six-month window | **$24,303**<br>three campaigns | **8.70x**<br>$211,392.24 ÷ $24,302.61 |

## What does reported ROAS prove, and what doesn't it?

| Verified by the ad dashboard | Not shown by the ad dashboard |
| :--- | :--- |
| Spend by campaign, to the cent | Product cost, shipping, and fulfillment |
| Purchase value Meta attributes to each campaign | Refunds, returns, and cancellations |
| Reported orders, add-to-carts, and average order value | Whether those buyers would have purchased anyway |
| The result across the full reporting window | Month-by-month consistency, unless monthly rows are shown |
| How campaigns compare inside one account | Profit after every cost of running the business |

*AEO note: Two-column "verified vs not shown" tables are among the formats AI answers lift most often. Each row is a complete, standalone claim.*

## Is dashboard "net profit" real profit?

No. In many ad dashboards, the field labeled Net Profit is simply attributed sales minus ad spend. For the account above that is $187,089.63. It is not business profit, because it excludes product cost, fulfillment, refunds, overhead, and taxes. Reporting it as profit overstates the result.

## How should you read ROAS across campaigns?

By job, not by ranking. Campaigns in one account do different work, so their ROAS should differ.

| Campaign | Job | Reported ROAS |
| :--- | :--- | :--- |
| Advantage+ Shopping | Match shoppers to catalog products and scale demand | 9.89x |
| Retargeting | Bring back people who already showed intent. Highest average order value. | 6.20x |
| Evergreen | Keep the brand live beyond the primary campaign | 4.52x |
| **Whole account** | Blended result | **8.70x** |

Advantage+ Shopping used 74.3% of spend and produced 84.5% of attributed sales, so budget was concentrated where the reported results were strongest. Evergreen's lower ROAS is not a failure. It is doing a different job.

## How should agencies report ROAS honestly?

1. **Name the source.** Say "Meta-attributed" or "platform-reported" every time the number appears.
2. **State the window.** A six-month result is not proof that every month performed the same.
3. **Compare like with like.** The same event a year apart is a fair comparison. One retailer went from 17.2x to about 35.9x on the same national event, on 2.6% less spend.
4. **Show what is not shown.** Put the limits next to the result, not in a footnote nobody reads.
5. **Never invent the missing data.** If monthly rows or margins are not in the source, the claim stops where the source stops.

## Frequently asked questions

**What is a good ROAS?**
It depends on your margin. Break-even ROAS is 1 divided by your gross margin, so a product with a 40% margin needs 2.5x before the gross profit from ad-driven sales covers the ad spend. A good ROAS clears that line with room left for every other cost.

**Why does Meta report different sales than Shopify?**
They count differently. Meta credits purchases to ads using its attribution window and modeling, including some conversions it estimates. Your store records actual orders. The two will rarely match, and neither is wrong. They answer different questions.

**Is a higher ROAS always better?**
No. Very high ROAS can mean a campaign is only reaching people who would have bought anyway, or that budget is too small to find new buyers. Read ROAS beside new-customer volume and total profit, not alone.

---

## Behind the page: how this sample is built for answer engines

| Technique | Where it shows up in this sample |
| :--- | :--- |
| Definitional target | The page aims to be the source for a "what is" question, the prompt type answer engines most often answer by quoting one page. |
| Answer-first | The short answer defines the term, says what it proves, and says what it does not, in 60 words. |
| Checkable math | Every derived figure (8.70x, $187,089.63, 74.3%, 84.5%) is shown with its inputs, so a model or a skeptical reader can verify it. |
| Misconception correction | A dedicated section corrects the dashboard "net profit" misread. Pages that correct common errors are frequently cited in AI answers. |
| Extractable formats | One formula, three stat tiles, two tables, one numbered list, three FAQs. |
| Consistency | Figures match the source case study exactly. ROAS for the year-over-year example is rounded, not truncated. |

<details>
<summary>Schema markup (JSON-LD)</summary>

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Article",
      "headline": "What does Meta ROAS actually prove?",
      "description": "What Meta-reported ROAS verifies, what it cannot show, and how to report it honestly, with a worked six-month example.",
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
          "name": "What is a good ROAS?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "It depends on your margin. Break-even ROAS is 1 divided by your gross margin, so a product with a 40% margin needs 2.5x before the gross profit from ad-driven sales covers the ad spend. A good ROAS clears that line with room left for every other cost."
          }
        },
        {
          "@type": "Question",
          "name": "Why does Meta report different sales than Shopify?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "They count differently. Meta credits purchases to ads using its attribution window and modeling, including some conversions it estimates. Your store records actual orders. The two will rarely match, and neither is wrong. They answer different questions."
          }
        },
        {
          "@type": "Question",
          "name": "Is a higher ROAS always better?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "No. Very high ROAS can mean a campaign is only reaching people who would have bought anyway, or that budget is too small to find new buyers. Read ROAS beside new-customer volume and total profit, not alone."
          }
        }
      ]
    }
  ]
}
```

</details>

---

*Writing sample by Justin Mitchiner. Built from an anonymized six-month e-commerce account and a year-over-year event campaign. Sales, orders, and ROAS are Meta-reported attribution measures, not independently audited cash revenue, fulfilled orders, or profit. Results vary by offer, product economics, tracking, creative, and execution.*

[← All writing samples](README.md)
