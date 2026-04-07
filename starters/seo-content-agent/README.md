# SEO Content Agent

Build a research-to-brief-to-draft system for publishing content that targets search demand with less manual busywork.

## What you are building

This starter is for a workflow that takes a topic, keyword cluster, or content gap and turns it into a production-ready content asset. The system should gather search intent, inspect competing pages, build a brief, draft the article, and prepare clean handoff notes for an editor or publishing workflow.

The point is not to generate bland content at scale. The point is to compress the messy research and briefing work that slows content teams down.

## Who should build it

- SEO consultants
- content teams
- affiliate site operators
- agencies
- SaaS growth teams

This starter is strongest when the user already cares about speed, editorial consistency, and repeatable briefing quality.

## End-to-end workflow

1. Accept a keyword, topic cluster, or content gap.
2. Pull search results and competing pages.
3. Identify search intent, common structures, and weak spots in the SERP.
4. Generate a content brief with outline, angle, FAQs, and internal-link opportunities.
5. Draft the article using the approved brief.
6. Run quality checks before handoff or publishing.

## Inputs and outputs

Inputs:

- primary keyword or topic cluster
- target audience
- brand voice
- existing pages to avoid overlap
- output format or CMS destination

Outputs:

- keyword cluster
- content brief
- outline
- article draft
- optimization notes
- internal-link suggestions

## How to build the MVP

Treat briefing and drafting as two separate products. That alone makes the workflow dramatically more usable.

### MVP shape

1. Start with a keyword intake form.
2. Pull a small SERP snapshot and the top competing pages.
3. Build a briefing layer that extracts:
   search intent, angle, headings, FAQs, and gaps.
4. Save the brief as a structured object.
5. Draft only after the brief exists.
6. Run a QA layer for:
   unsupported claims, overlap risk, thin sections, and missing FAQs.
7. Hand off the output to Notion or your CMS instead of auto-publishing.

## Core system components

- topic intake
- SERP collector
- competitor page extractor
- brief generator
- drafting agent
- editorial QA layer
- handoff destination such as Notion or CMS

## Recommended API stack

- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for SERP discovery
- [Google Keyword Scraper](https://apify.com/dxbear/google-keyword-scraper?fpr=p2hrc6) for keyword expansion and opportunity finding
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for competitor-page extraction
- OpenAI and Notion or your CMS API for brief generation, drafting, and handoff

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Add editor review before anything is published. The most important checks are:

- factual accuracy
- search-intent match
- duplicate-topic risk
- brand voice alignment
- legal, medical, or financial sensitivity

## What a strong v1 looks like

A strong v1 gives an editor three things:

- a clear angle
- a clear structure
- a draft that is worth editing instead of rewriting

If the workflow still produces vague outlines and generic drafts, the real bottleneck is probably the brief, not the writing model.

## Monetization ideas

- agency content production systems
- niche SEO briefing tools
- editorial copilots for content teams
- productized "brief plus draft" services for founders and operators

## Fastest path to v1

1. Topic intake
2. SERP snapshot
3. Brief generation
4. Draft generation
5. Editorial QA

That sequence gives you a real content pipeline without overbuilding publishing automation too early.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

