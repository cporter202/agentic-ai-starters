# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| Firecrawl | pricing-page, product-page, and changelog extraction | Reliable input for change detection |
| Similarweb | traffic and referral context | Adds directional market signal beyond page copies |
| BuiltWith | technology stack monitoring | Helpful when product or infrastructure changes matter strategically |
| OpenAI | change interpretation and briefing | Converts deltas into readable intel and next steps |

## Optional alternatives

- Tavily: useful for broader web research around launches and press.
- Apify: useful for collecting additional public-source signals on a schedule.
- Anthropic: useful for long-form review or a second-opinion memo.

## Suggested stack tiers

- Lean stack: Firecrawl + OpenAI.
- Best-value stack: Firecrawl + Similarweb + OpenAI.
- Premium stack: Firecrawl + Similarweb + BuiltWith + OpenAI + Langfuse.
