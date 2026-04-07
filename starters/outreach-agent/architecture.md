# Architecture

## Core components

- lead intake and suppression rules
- enrichment and personalization layer
- copy-generation agent
- sequence scheduler
- reply classifier and human handoff queue
- deliverability and logging layer

## Suggested flow

1. Validate the lead list and remove suppressed records.
2. Collect enough company and role context for message relevance.
3. Draft personalized first-touch and follow-up messages.
4. Schedule a sequence with stop conditions for replies or errors.
5. Classify replies and route positive signals to a human closer.

## MVP notes

- Keep sending, copy generation, and reply handling separate.
- Add hard suppression rules for unsubscribes, bounces, and competitors.
- Require human approval for high-value accounts until the workflow proves itself.
