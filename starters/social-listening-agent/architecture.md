# Architecture

## Core components

- source connectors for social and web feeds
- normalization layer for noisy text and metadata
- topic clustering and sentiment pipeline
- alerting engine with urgency rules
- digest generator for weekly or daily summaries
- review layer for brand-risk events

## Suggested flow

1. Pull recent items by account, keyword, or competitor.
2. Standardize text, timestamps, author data, and engagement fields.
3. Classify each item by topic, sentiment, and urgency.
4. Group related mentions into narratives and trend summaries.
5. Route urgent events to Slack or email, and send recap reports on schedule.

## MVP notes

- Start with a few high-signal sources rather than chasing total coverage.
- Store raw posts alongside normalized summaries for auditability.
- Add allowlists and blocklists so the agent ignores obvious spam.
