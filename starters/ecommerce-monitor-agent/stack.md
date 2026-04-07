# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| Shopify Admin API | owned-store catalog and product signals | Best anchor when the workflow supports a Shopify operator |
| Amazon Selling Partner API | seller and marketplace operations | Useful for marketplace-aware monitoring and reporting |
| Firecrawl | competitor product-page extraction | Good fit for repeatable product and price snapshots |
| OpenAI | summarization, anomaly triage, operator recommendations | Turns raw deltas into actions teams can actually use |

## Optional alternatives

- Apify: useful for broader competitor collection and recurring crawling jobs.
- SerpApi: useful for shopping-result monitoring or brand query checks.
- Anthropic: useful for long-form review analysis or second-pass QA.

## Suggested stack tiers

- Lean stack: Shopify Admin API + Firecrawl + OpenAI.
- Best-value stack: Shopify Admin API + Amazon Selling Partner API + Firecrawl + OpenAI.
- Premium stack: Shopify Admin API + Amazon Selling Partner API + Firecrawl + OpenAI + Langfuse.
