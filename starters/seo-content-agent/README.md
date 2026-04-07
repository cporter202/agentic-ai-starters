# SEO Content Agent

Build a research-to-brief-to-draft system for publishing content that targets search demand with less manual busywork.

## What it does

This starter takes a topic cluster or keyword target, analyzes search intent and competing pages, creates a content brief, drafts an article, and prepares optimization notes for editors or publishers.

## Who it is for

- SEO consultants
- content teams
- affiliate site operators
- agencies
- SaaS growth teams

## Workflow

1. Start from a topic, keyword set, or content gap.
2. Collect SERP context, competitor pages, and search intent patterns.
3. Build a brief with angle, structure, and internal-link opportunities.
4. Draft the piece and run quality checks.
5. Hand off to an editor, CMS, or publishing pipeline.

## Inputs and outputs

Inputs: target keyword, site positioning, audience, brand voice, existing URLs.

Outputs: keyword cluster, content brief, article draft, on-page optimization notes, internal link suggestions.

## Recommended API stack

- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for SERP discovery
- [Google Keyword Scraper](https://apify.com/dxbear/google-keyword-scraper?fpr=p2hrc6) for keyword expansion and opportunity finding
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for competitor-page extraction
- OpenAI and Notion or your CMS API for brief generation, drafting, and handoff

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

SEO teams often spend too much time moving between research, outlining, drafting, and QA. This workflow can shorten the cycle without turning content into generic sludge.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
