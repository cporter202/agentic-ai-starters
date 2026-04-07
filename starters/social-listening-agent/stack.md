# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| X API | post, mention, and account monitoring | Useful for real-time public conversation tracking |
| YouTube Data API | video and comment monitoring | Strong fit for creator, product, and review ecosystems |
| SerpApi | news and search collection | Adds wider web context around spikes or brand events |
| OpenAI | classification, clustering, summarization, alert drafting | Turns noisy streams into operator-ready insight |

## Optional alternatives

- Reddit API: useful when community discussions are a major source of signal.
- Apify: useful for broader coverage of channels or directories without strong native APIs.
- Anthropic: useful for a second-pass reviewer on sensitive escalations.

## Suggested stack tiers

- Lean stack: X API + OpenAI.
- Best-value stack: X API + YouTube Data API + OpenAI.
- Premium stack: X API + YouTube Data API + SerpApi + OpenAI + Langfuse.
