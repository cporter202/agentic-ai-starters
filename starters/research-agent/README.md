# Research Agent

Build a citation-first research assistant that turns a topic, company, or market question into a usable brief.

## What you are building

This starter is for a research workflow that behaves more like an analyst than a chatbot. The system takes a scoped brief, expands it into research tasks, collects source material, extracts evidence, organizes claims by theme, and returns a memo with citations, confidence notes, and follow-up questions.

The product works well as:

- an internal research copilot
- an agency deliverable engine
- a paid market-intelligence workflow
- a founder tool for fast due diligence

## Who should build it

- analysts
- founders
- agencies
- consultants
- product and strategy teams

This starter is especially strong if your users already spend hours collecting articles, summarizing competitor information, or producing recurring reports.

## End-to-end workflow

1. Accept a research brief, topic, company list, or market question.
2. Turn that request into a structured research plan with search angles and priority questions.
3. Search the web and collect high-signal sources.
4. Crawl the selected pages and extract key evidence.
5. Deduplicate claims, cluster evidence by theme, and score confidence.
6. Generate a memo with citations, unresolved questions, and recommended next actions.
7. Route low-confidence or contradictory findings for human review.

## Inputs and outputs

Inputs:

- research question
- target companies or domains
- industries and regions
- date range or recency rules
- output format such as memo, brief, or comparison table

Outputs:

- executive summary
- source table
- evidence-backed findings
- citation links
- confidence notes
- open questions
- recommended next actions

## How to build the MVP

Start with a narrow use case such as company research, market scans, or competitor brief generation. Do not begin with a fully open-ended "research anything" product.

### MVP shape

1. Create a simple intake form with:
   research brief, source constraints, date range, and desired output format.
2. Add a planner step that converts the brief into:
   search queries, must-answer questions, target entities, and stop conditions.
3. Build a retrieval step that:
   searches, selects candidate pages, and saves raw source metadata.
4. Add an extraction step that:
   pulls title, publication date, claims, supporting evidence, and quote-worthy facts.
5. Store evidence separately from the final answer so you can re-run synthesis cheaply.
6. Add a synthesis step that:
   writes the report only from saved evidence, not from memory.
7. Add one final review layer that blocks uncited claims from the final memo.

## Core system components

- Intake UI or API endpoint for research briefs
- Planner agent for query generation and scope control
- Retrieval layer for discovery and source collection
- Extraction layer for page parsing and fact capture
- Evidence store for claims, citations, and confidence
- Synthesis agent for brief generation
- Review layer for conflicts, stale sources, and unsupported claims

## Recommended API stack

- [AI Web Research Agent](https://apify.com/devwithbobby/ai-web-research-agent?fpr=p2hrc6) for end-to-end research runs
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for crawling and extracting source material
- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for discovery and search expansion
- OpenAI for planning, extraction, synthesis, and structured outputs

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Do not make this fully autonomous on day one. Add human checkpoints for:

- uncited findings
- conflicting sources
- high-stakes claims
- outdated source material
- sensitive industries such as finance, health, or legal workflows

## What a strong v1 looks like

A strong v1 does not need a big UI. It needs:

- reliable citations
- repeatable source collection
- saved evidence objects
- fast re-generation of briefs
- a clear output format users can trust

If you get those right, you can later add dashboards, saved companies, recurring jobs, and team collaboration.

## Monetization ideas

- sell recurring competitor briefs to agencies or consultants
- offer vertical research reports for SaaS, ecommerce, or local markets
- build an internal intelligence tool for founders or operators
- productize due-diligence workflows for investors or recruiters

## Fastest path to v1

If you want the fastest possible first version, build this in order:

1. Brief intake
2. Search and crawl
3. Evidence extraction
4. Citation-based synthesis
5. Human approval

That sequence gets you to a useful product much faster than trying to build memory, collaboration, and dashboards too early.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

