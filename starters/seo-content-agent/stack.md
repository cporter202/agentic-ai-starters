# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| SerpApi | SERP collection and keyword context | Gives the agent real search-result signals instead of guessing intent |
| Firecrawl | competitor page extraction | Helps the briefing layer compare headings, topics, and page structure |
| OpenAI | outlining, drafting, editing, structured QA | Strong fit for multi-step content workflows |
| Notion API | editorial handoff and review workflows | Useful for teams that want human approval before publish |

## Optional alternatives

- Tavily: a lighter search option when broad web context matters more than exact SERPs.
- Anthropic: useful for long-form review or style-sensitive editing passes.
- Apify: useful for niche content-source scraping or recurring collection jobs.

## Suggested stack tiers

- Lean stack: SerpApi + OpenAI + Notion API.
- Best-value stack: SerpApi + Firecrawl + OpenAI + Notion API.
- Premium stack: SerpApi + Firecrawl + OpenAI + Anthropic + Langfuse.
