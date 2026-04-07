# Real Estate Agent

Build a property intelligence workflow that monitors listings, enriches neighborhood context, and helps operators evaluate opportunities faster.

## What it does

This starter pulls listing and rent data, monitors target markets, summarizes nearby amenities and risk factors, and turns raw property information into acquisition or operating insight.

## Who it is for

- real estate investors
- wholesalers
- brokers
- acquisition teams
- property research operators

## Workflow

1. Define markets, buy box, and underwriting assumptions.
2. Collect listings, rent estimates, and neighborhood context.
3. Score properties for fit and investigate notable deltas.
4. Generate operator notes, comps, and follow-up tasks.
5. Route top opportunities to a human review pipeline.

## Inputs and outputs

Inputs: target markets, price range, property type, strategy, rent assumptions.

Outputs: ranked properties, comp notes, market snapshots, underwriting summaries, alert feed.

## Recommended API stack

- [Zillow Scraper](https://apify.com/mido_99/zillow-scraper?fpr=p2hrc6) for listing intelligence
- [Google Maps B2B Leads Scraper](https://apify.com/primeparse/google-maps-scraper?fpr=p2hrc6) for location and nearby-business context
- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for market and locality discovery
- RentCast, OpenAI, and Resend or Slack for underwriting notes, structured property data, and alerts

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Real estate workflows benefit from constant monitoring, structured comparison, and fast triage, which makes them a strong fit for autonomous agents with human approval.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
