# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| People Data Labs | company and person enrichment | Gives the workflow richer targeting and scoring data |
| Hunter | email discovery and verification | Keeps the final list usable for outbound |
| Google Places API | local business discovery | Strong fit for geo-based prospecting and local lead gen |
| OpenAI | scoring, segmentation, enrichment QA | Turns raw records into ranked and explainable opportunities |

## Optional alternatives

- Apify: useful for collecting leads from directories or vertical sites.
- Tavily: useful for web-based discovery when maps are not enough.
- Resend: useful if you want this starter to hand off directly into outbound delivery.

## Suggested stack tiers

- Lean stack: Google Places API + Hunter + OpenAI.
- Best-value stack: Google Places API + People Data Labs + Hunter + OpenAI.
- Premium stack: Apify + People Data Labs + Hunter + OpenAI + Langfuse.
