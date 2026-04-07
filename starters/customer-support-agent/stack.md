# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| Zendesk API | ticket ingestion and workflow state | Strong fit for support-first automation |
| Notion API | internal knowledge and SOP retrieval | Useful when teams store live operating guidance in docs |
| Slack API | escalation and internal alerts | Keeps humans in the loop for sensitive cases |
| OpenAI | classification, retrieval-aware drafting, summaries | Turns support data into faster and more consistent actions |

## Optional alternatives

- Anthropic: useful for second-pass response review or long-case synthesis.
- Resend: useful when support actions flow through email digests and summaries.
- GitHub API: useful when the support loop needs to create bug reports for product teams.

## Suggested stack tiers

- Lean stack: Zendesk API + OpenAI.
- Best-value stack: Zendesk API + Notion API + OpenAI + Slack API.
- Premium stack: Zendesk API + Notion API + Slack API + OpenAI + Langfuse.
