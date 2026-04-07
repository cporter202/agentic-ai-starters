# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| OpenAI | tool-aware reasoning and orchestration | Strong fit for structured tool calling and agent loops |
| GitHub API | repo reads, issues, PRs, and code workflow actions | One of the most common high-value tool surfaces for autonomous agents |
| Notion API | documentation reads and updates | Useful for operational memory and human-facing outputs |
| Slack API | approval routing and notifications | Helpful for keeping humans in the loop during tool use |

## Optional alternatives

- Tavily: useful for live web retrieval inside the same agent loop.
- Anthropic: useful for review-mode agents or second-pass checks.
- Resend: useful when the toolchain needs email-based reports or alerts.

## Suggested stack tiers

- Lean stack: OpenAI + GitHub API.
- Best-value stack: OpenAI + GitHub API + Notion API.
- Premium stack: OpenAI + Anthropic + GitHub API + Notion API + Slack API.
