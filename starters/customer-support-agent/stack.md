# Curated API Stack

## Featured APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) | help-center and docs ingestion | Great for building retrieval-ready support knowledge from public docs |
| [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) | structured extraction from support sites | Useful when docs are inconsistent and need prompt-based extraction |
| [Trustpilot Scraper](https://apify.com/happitap/trustpilot-scraper?fpr=p2hrc6) | customer-feedback ingestion | Adds external customer sentiment and complaint themes |
| [Reddit Posts & Comments Scraper](https://apify.com/parseforge/reddit-posts-comments-scraper?fpr=p2hrc6) | community support signals | Useful for support teams that monitor user frustration outside the ticket queue |

## Companion APIs

- OpenAI: classification, retrieval-aware drafting, and summaries.
- Zendesk API: ticket workflows.
- Slack API: internal escalation.

## Suggested stack tiers

- Lean stack: OpenAI + [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6).
- Best-value stack: OpenAI + Zendesk API + [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6).
- Premium stack: OpenAI + Zendesk API + [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) + [Trustpilot Scraper](https://apify.com/happitap/trustpilot-scraper?fpr=p2hrc6) + Langfuse.
