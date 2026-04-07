# Ecommerce Monitor Agent

Build a product and pricing intelligence workflow for stores, operators, and commerce agencies.

## What you are building

This starter is for a system that watches product listings, pricing, stock signals, reviews, and assortment changes across owned stores or competitor channels, then turns that raw data into operator-ready alerts.

The goal is not to collect endless product rows. The goal is to tell a team what changed, how important it is, and what action should happen next.

## Who should build it

- ecommerce brands
- marketplace operators
- pricing teams
- agencies
- Amazon and Shopify sellers

This starter is strongest when users care about price moves, stock changes, review trends, or competitor assortment changes.

## End-to-end workflow

1. Define the products, categories, stores, and competitors to monitor.
2. Pull recurring snapshots of listing data.
3. Normalize products and compare them against prior snapshots.
4. Detect material changes in price, stock, reviews, or assortment.
5. Summarize the changes in operator language.
6. Push alerts or reports to the people who need to act.

## Inputs and outputs

Inputs:

- tracked SKUs or product URLs
- competitors and marketplaces
- alert thresholds
- categories
- reporting cadence

Outputs:

- change feed
- price alerts
- stock alerts
- review summaries
- assortment changes
- recommended operator actions

## How to build the MVP

Pick one category and one competitor set first. The hardest part is entity matching and alert quality, not raw collection volume.

### MVP shape

1. Define a product registry with:
   product ID, store, URL, competitor labels, and alert thresholds.
2. Save recurring snapshots of:
   price, stock, title, reviews, and listing metadata.
3. Build a change-detection layer that compares:
   current snapshot versus prior snapshot.
4. Add a summarization layer that says:
   what changed, why it matters, and whether it needs action.
5. Send alerts only for meaningful deltas.
6. Add a dashboard or digest after the alerting quality is solid.

## Core system components

- product registry
- snapshot collector
- normalization pipeline
- change-detection service
- review summarizer
- alerting and reporting layer

## Recommended API stack

- [Amazon Product Scraper](https://apify.com/get-leads/amazon-product-scraper?fpr=p2hrc6) for marketplace product, price, and review monitoring
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for competitor store crawling
- [Trustpilot Scraper](https://apify.com/happitap/trustpilot-scraper?fpr=p2hrc6) for review and reputation monitoring
- Shopify Admin API and OpenAI for owned-store sync, summarization, and operator alerts

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Keep people in the loop for:

- large price swings
- suspicious inventory changes
- mismatched competitor product mapping
- reputation spikes that need manual interpretation
- high-value products with revenue impact

## What a strong v1 looks like

A strong v1 makes it easy to answer:

- which competitor changed price first?
- which products are low on stock?
- which review themes are getting worse?
- what should the team look at right now?

If the user still has to inspect every raw listing manually, the workflow is not finished.

## Monetization ideas

- competitor monitoring for ecommerce agencies
- marketplace alerting for sellers
- category intelligence dashboards
- productized pricing-watch services

## Fastest path to v1

1. Track one category
2. Save daily snapshots
3. Detect changes
4. Summarize material deltas
5. Send one daily alert digest

That is enough to create a useful operator workflow before building a bigger dashboard product.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
