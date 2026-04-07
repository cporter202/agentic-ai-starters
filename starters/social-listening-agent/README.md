# Social Listening Agent

Build an always-on listening workflow that tracks brand mentions, competitor chatter, recurring complaints, and emerging narratives.

## What it does

This starter collects posts, comments, videos, and web chatter from selected sources, clusters the conversation into themes, highlights sentiment shifts, and produces alerting and reporting outputs.

## Who it is for

- brand teams
- agencies
- founders
- product marketers
- community managers

## Workflow

1. Define tracked brands, products, competitors, and keywords.
2. Collect posts and content from supported channels.
3. Normalize noisy text and cluster by topic.
4. Score urgency, sentiment, and trend movement.
5. Send alerts and weekly insight summaries.

## Inputs and outputs

Inputs: keyword set, brand list, competitor list, channels, alert rules.

Outputs: mention feed, theme clusters, sentiment summaries, crisis alerts, weekly recap.

## Recommended API stack

Use the X API and YouTube Data API for channel coverage, add Google-based news or search collection for broader context, and use OpenAI for classification, summarization, and escalation logic. See [`stack.md`](./stack.md) for the featured Apify picks and tracked direct links.

## Why build it

Social listening becomes much more valuable when it moves beyond dashboards and starts prioritizing what a team should respond to right now.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
