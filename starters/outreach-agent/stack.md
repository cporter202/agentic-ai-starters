# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| People Data Labs | contact and company enrichment | Improves targeting and personalization quality |
| Hunter | email discovery and verification | Helps reduce wasted sends and bad records |
| Resend | outbound delivery and workflow handoff | Simple transactional delivery layer for agent-driven sequences |
| OpenAI | personalization, sequence writing, reply classification | Turns contact context into relevant outbound actions |

## Optional alternatives

- Firecrawl: useful for pulling website context and recent company signals.
- Apify: useful for collecting lead context from directories or public pages.
- Anthropic: useful for second-pass quality review on higher-value sequences.

## Suggested stack tiers

- Lean stack: Hunter + Resend + OpenAI.
- Best-value stack: People Data Labs + Hunter + Resend + OpenAI.
- Premium stack: People Data Labs + Hunter + Firecrawl + Resend + OpenAI + Langfuse.
