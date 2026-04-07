# Competitor Intel Agent

Build a system that watches competitors and turns their public moves into strategic updates instead of random tabs in a browser.

## What you are building

This starter is for a recurring competitive-intelligence workflow. It should monitor pricing pages, product pages, launches, messaging shifts, hiring signals, and related public sources, then turn that activity into a readable brief with implications.

The best version of this product is less about "scraping competitors" and more about building an institutional memory of their moves over time.

## Who should build it

- SaaS founders
- product marketers
- strategy teams
- agencies
- B2B operators

This starter works best when users already review competitors manually and want a consistent way to track changes over weeks and months.

## End-to-end workflow

1. Define the competitor set and watch surfaces.
2. Save baseline snapshots for key pages and public channels.
3. Revisit those sources on a schedule.
4. Detect meaningful changes in messaging, pricing, launches, or activity.
5. Add interpretation and likely implications.
6. Ship recurring strategy briefs or alerts.

## Inputs and outputs

Inputs:

- competitor list
- key URLs
- watch rules
- reporting cadence
- optional strategic focus such as pricing or messaging

Outputs:

- change log
- launch watchlist
- messaging summary
- pricing deltas
- strategic brief
- follow-up questions

## How to build the MVP

Start with a focused watchlist. Five useful competitors with reliable tracking is better than fifty noisy ones.

### MVP shape

1. Create a competitor registry with:
   company name, website, pricing URL, product URL, changelog URL, and optional launch channels.
2. Save a baseline snapshot for each important surface.
3. Re-crawl those surfaces on a schedule.
4. Compute deltas in:
   page copy, page structure, pricing blocks, and launch mentions.
5. Add a synthesis step that explains:
   what changed and why it may matter.
6. Deliver a weekly brief before adding real-time alerting.

## Core system components

- competitor registry
- snapshot collector
- page diffing layer
- launch and activity collector
- synthesis agent
- scheduled report generator

## Recommended API stack

- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for monitoring pricing pages, product pages, and changelogs
- [Product Hunt Scraper](https://apify.com/vulnv/producthunt-scraper?fpr=p2hrc6) for launch tracking
- [LinkedIn Company Posts Scraper](https://apify.com/data-slayer/linkedin-company-posts-scraper?fpr=p2hrc6) for messaging and campaign monitoring
- OpenAI, Similarweb, and BuiltWith for interpretation, traffic context, and technology shifts

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Review should happen when:

- a pricing change could trigger a strategic response
- a launch signal is ambiguous
- traffic or hiring data is weak and over-interpretation is likely
- a summary includes major strategic inference

## What a strong v1 looks like

A strong v1 tells the operator:

- what changed
- how recent it is
- where it happened
- why it might matter
- what to watch next

That is far more useful than a dump of page diffs.

## Monetization ideas

- competitive monitoring for agencies
- paid intelligence digests for founders
- vertical market watch products
- internal strategy tooling for product and marketing teams

## Fastest path to v1

1. Track a small competitor set
2. Save baseline snapshots
3. Re-run on a schedule
4. Compute meaningful deltas
5. Generate a weekly memo

That gets you to a valuable strategy product much faster than trying to build a full intelligence platform at once.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

