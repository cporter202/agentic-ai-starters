# Curated API Stack

## Primary recommended APIs

| API | Used for | Why it belongs |
| --- | --- | --- |
| OpenAI | planner, worker, and tool-using agent roles | Flexible core model layer for structured multi-step work |
| Anthropic | reviewer or long-context specialist roles | Useful for cross-checking and second-pass reasoning |
| Trigger.dev | orchestration, retries, schedules, background runs | Strong fit for durable multi-step agent workflows |
| Langfuse | traces, evaluations, and debugging | Helps teams understand where multi-agent systems fail or drift |

## Optional alternatives

- Slack API: useful for approvals, escalation, and operator notifications.
- GitHub API: useful when the workflow executes code or issue-management tasks.
- Notion API: useful for shared memory, SOP storage, and human-facing reports.

## Suggested stack tiers

- Lean stack: OpenAI + Trigger.dev.
- Best-value stack: OpenAI + Trigger.dev + Langfuse.
- Premium stack: OpenAI + Anthropic + Trigger.dev + Langfuse + Slack API.
