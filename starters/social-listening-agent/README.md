# Social Listening Agent

Build an always-on listening workflow that tracks brand mentions, competitor chatter, recurring complaints, and emerging narratives.

## What you are building

This starter is for a system that watches selected public channels, collects posts and discussions, clusters the noise into useful themes, and routes the highest-signal events into alerts or recurring summaries.

The product should not feel like a dashboard full of random mentions. It should feel like an operator assistant that tells a team what matters, why it matters, and what to do next.

## Who should build it

- brand teams
- agencies
- founders
- product marketers
- community managers

This starter is especially useful when users care about launches, reputation, complaints, community trends, or competitor narrative shifts.

## End-to-end workflow

1. Define tracked keywords, brands, products, and competitors.
2. Collect posts, comments, and public mentions from selected channels.
3. Normalize the text and metadata.
4. Classify items by theme, sentiment, urgency, and response need.
5. Cluster related chatter into narratives.
6. Send alerts for urgent items and summaries for recurring reporting.

## Inputs and outputs

Inputs:

- tracked brands
- competitors
- keywords and exclusions
- selected channels
- alert thresholds
- reporting cadence

Outputs:

- mention feed
- topic clusters
- sentiment summaries
- urgent alerts
- weekly recap
- recommended response actions

## How to build the MVP

Do not start with full channel coverage. Start with the two channels that matter most and build the classification and alerting loop first.

### MVP shape

1. Add a tracking configuration for:
   brands, competitor names, product names, and keyword groups.
2. Pull content from one or two public sources on a schedule.
3. Normalize every item into one schema:
   source, author, timestamp, text, URL, engagement, and raw content.
4. Add a classification step for:
   topic, sentiment, urgency, and response-needed.
5. Build a clustering step that groups repetitive mentions into narratives.
6. Send alerts only when:
   urgency is high or the narrative is growing quickly.
7. Generate one daily or weekly recap for operator review.

## Core system components

- tracking configuration layer
- source connectors
- normalization pipeline
- classification and sentiment layer
- narrative clustering
- alerting engine
- digest generator

## Recommended API stack

- [Twitter/X Scraper](https://apify.com/automation-lab/twitter-scraper?fpr=p2hrc6) for public post monitoring
- [YouTube Comments Scraper](https://apify.com/apidojo/youtube-comments-scraper?fpr=p2hrc6) for comment and audience sentiment
- [Reddit Posts & Comments Scraper](https://apify.com/parseforge/reddit-posts-comments-scraper?fpr=p2hrc6) for community signal capture
- OpenAI and Slack for classification, summarization, and alert routing

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Require human review for:

- crisis-like spikes
- ambiguous sarcasm or humor
- policy-sensitive brand issues
- complaints that could trigger refunds or legal escalation
- competitor narratives that require strategic interpretation

## What a strong v1 looks like

A strong v1 should save the user time by answering:

- what changed this week?
- what is getting louder?
- what needs a response?
- which complaints are repeating?

That is much more valuable than simply dumping mentions into a feed.

## Monetization ideas

- social monitoring for agencies
- reputation alerting for ecommerce brands
- launch monitoring for startups and creators
- competitive narrative tracking for B2B companies

## Fastest path to v1

1. Track a small keyword set
2. Pull from two channels
3. Classify and cluster
4. Alert on high urgency
5. Send recap summaries

That is enough to create a useful monitoring product before you expand source coverage.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
