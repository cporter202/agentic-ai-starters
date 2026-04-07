# Curated API Stack

## Featured APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| [AI Web Research Agent](https://apify.com/devwithbobby/ai-web-research-agent?fpr=p2hrc6) | specialist research worker | Useful as a dedicated worker inside a larger multi-agent flow |
| [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) | flexible extraction worker | Good fit for agents that need structured outputs from arbitrary sites |
| [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) | knowledge and docs worker | Strong input layer for retrieval-heavy agent teams |
| [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) | live-search worker | Helps planner agents assign discovery tasks quickly |

## Companion APIs

- OpenAI: planner, worker, and tool-using roles.
- Anthropic: reviewer roles and long-context checks.
- Trigger.dev: orchestration, retries, and schedules.
- Langfuse: traces, evaluations, and debugging.

## Suggested stack tiers

- Lean stack: OpenAI + [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) + Trigger.dev.
- Best-value stack: OpenAI + [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) + Trigger.dev + Langfuse.
- Premium stack: OpenAI + Anthropic + [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) + [AI Web Research Agent](https://apify.com/devwithbobby/ai-web-research-agent?fpr=p2hrc6) + Langfuse.
