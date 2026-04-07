# Research Agent

Build a citation-first research assistant that turns a topic, company, or market question into a usable brief.

## What it does

This starter plans a research run, gathers web sources, extracts evidence, scores source quality, and produces a final memo with citations and recommended next actions.

## Who it is for

- analysts
- founders
- agencies
- consultants
- product and strategy teams

## Workflow

1. Accept a research brief, topic, or company list.
2. Expand the brief into search angles and hypotheses.
3. Search, crawl, and extract relevant source material.
4. Deduplicate claims and score evidence quality.
5. Draft a structured brief with citations and confidence notes.
6. Route unclear claims for human review.

## Inputs and outputs

Inputs: research question, target companies, industries, regions, date range, output format.

Outputs: research memo, source table, key claims, open questions, next-step recommendations.

## Recommended API stack

- [AI Web Research Agent](https://apify.com/devwithbobby/ai-web-research-agent?fpr=p2hrc6) for end-to-end research runs
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for crawling and extracting source material
- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for discovery and search expansion
- OpenAI for synthesis, extraction, and final report generation

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Research is still one of the highest-value AI workflows because the work is repetitive, source-heavy, and easy to package into briefs, premium reports, internal copilots, or client deliverables.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
