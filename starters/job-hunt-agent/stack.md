# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| Adzuna API | job discovery and market data | Good foundation for collecting normalized listing data |
| Firecrawl | employer and listing-page extraction | Useful for richer context on companies and openings |
| OpenAI | fit scoring, tailored application assets, reminders | Strong fit for candidate-specific personalization |
| Notion API | search tracking and pipeline management | Makes it easy to keep humans in the loop |

## Optional alternatives

- SerpApi: useful for broader job-search coverage.
- Resend: useful when the workflow includes automated follow-up drafts or sends.
- Anthropic: useful for long-form application review or interview-prep simulations.

## Suggested stack tiers

- Lean stack: Adzuna API + OpenAI.
- Best-value stack: Adzuna API + Firecrawl + OpenAI + Notion API.
- Premium stack: Adzuna API + SerpApi + OpenAI + Notion API + Langfuse.
