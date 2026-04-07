# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| OpenAI | planning, extraction, synthesis, report generation | Strong fit for multi-step research loops and structured outputs |
| Tavily | live search and result retrieval | Fast way to turn research plans into web discovery runs |
| Firecrawl | clean page extraction and markdown output | Makes downstream evidence extraction more reliable |
| Langfuse | tracing, evaluation, prompt versioning | Helpful once research workflows become multi-step and client-facing |

## Optional alternatives

- Exa: good when semantic web search quality matters more than general breadth.
- Anthropic: useful when you want a second-model reviewer for higher-stakes briefs.
- Apify: useful when the workflow depends on niche web sources or repeated scraping jobs.

## Suggested stack tiers

- Lean stack: OpenAI + Tavily + SQLite or Postgres.
- Best-value stack: OpenAI + Tavily + Firecrawl + Postgres.
- Premium stack: OpenAI + Anthropic + Exa + Firecrawl + Langfuse.
