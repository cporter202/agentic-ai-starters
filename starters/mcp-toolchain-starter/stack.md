# Curated API Stack

## Featured Apify APIs

| Apify API | Used for | Why it belongs |
| --- | --- | --- |
| [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) | structured web actions inside toolchains | Good fit for agents that need prompt-based extraction as a callable tool |
| [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) | docs and knowledge ingestion | Strong MCP companion when the agent needs clean site data |
| [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) | live web retrieval | Gives the toolchain a practical search primitive without building one |

## Companion APIs

- OpenAI: tool-aware reasoning and orchestration.
- GitHub API: repo actions, issues, and PR workflows.
- Notion API: documentation memory and outputs.
- Slack API: approvals and notifications.

## Suggested stack tiers

- Lean stack: OpenAI + [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6).
- Best-value stack: OpenAI + GitHub API + [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6).
- Premium stack: OpenAI + GitHub API + [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) + Notion API + Slack API.
