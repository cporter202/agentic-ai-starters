# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| RentCast API | listing, rent, and property data | Strong base layer for property-focused workflows |
| Google Places API | amenity and neighborhood enrichment | Helps the agent explain location context, not just property stats |
| OpenAI | screening notes, comp summaries, operator packets | Useful for converting data into decision-ready output |
| Resend | alert delivery and summary reports | Lightweight way to ship shortlists and market updates |

## Optional alternatives

- Firecrawl: useful for collecting extra listing-page details from niche sites.
- Anthropic: useful for second-pass review on longer investment memos.
- Slack API: useful when the workflow lives inside an acquisition team.

## Suggested stack tiers

- Lean stack: RentCast API + OpenAI.
- Best-value stack: RentCast API + Google Places API + OpenAI + Resend.
- Premium stack: RentCast API + Google Places API + Firecrawl + OpenAI + Langfuse.
