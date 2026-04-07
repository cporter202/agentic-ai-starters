# Architecture

## Core components

- intake layer for briefs, topics, and filters
- planner agent that expands the brief into research tasks
- search layer for discovery across web and API sources
- extraction layer for article text, metadata, and structured facts
- evidence store for claims, citations, and confidence scoring
- synthesis agent for briefs, summaries, and action items
- review step for low-confidence or conflicting claims

## Suggested flow

1. Normalize the request into a structured research plan.
2. Run search queries by topic, company, and competitor angle.
3. Crawl the most promising sources and extract structured notes.
4. Group evidence by theme and remove duplicate claims.
5. Generate a memo with citations, uncertainty flags, and follow-up paths.

## MVP notes

- Start with one planner, one researcher, and one synthesis agent.
- Store evidence separately from final outputs so you can re-run synthesis cheaply.
- Add a mandatory citation check before publishing any final answer.
