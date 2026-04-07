# Ecommerce Monitor Agent

Build a product and pricing intelligence workflow for stores, operators, and commerce agencies.

## What it does

This starter watches product listings, pricing, stock signals, reviews, and assortment changes across your store, marketplaces, or selected competitors, then turns that data into alerts and action items.

## Who it is for

- ecommerce brands
- marketplace operators
- pricing teams
- agencies
- Amazon and Shopify sellers

## Workflow

1. Define stores, product sets, marketplaces, and tracking rules.
2. Collect catalog, pricing, and review data on a schedule.
3. Detect changes in price, availability, rating trends, or assortment.
4. Summarize material shifts and recommend next actions.
5. Push alerts to operators or dashboards.

## Inputs and outputs

Inputs: product URLs, SKUs, competitor list, alert thresholds, categories.

Outputs: change feed, price alerts, stock alerts, review summaries, operator recommendations.

## Recommended API stack

- [Amazon Product Scraper](https://apify.com/get-leads/amazon-product-scraper?fpr=p2hrc6) for marketplace product, price, and review monitoring
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for competitor store crawling
- [Trustpilot Scraper](https://apify.com/happitap/trustpilot-scraper?fpr=p2hrc6) for review and reputation monitoring
- Shopify Admin API and OpenAI for owned-store sync, summarization, and operator alerts

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Operators care less about raw scraped rows and more about fast answers to questions like what changed, how important it is, and what to do next.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
