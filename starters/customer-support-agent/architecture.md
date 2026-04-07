# Architecture

## Core components

- support-channel connector
- ticket classification layer
- knowledge retrieval layer
- reply-generation agent
- escalation and approval rules
- reporting and resolution analytics

## Suggested flow

1. Pull the latest support items with account context.
2. Classify intent, urgency, and whether the issue can be automated safely.
3. Retrieve knowledge snippets or prior solved tickets.
4. Draft a reply or next-step recommendation.
5. Escalate sensitive cases and log outcomes for review.

## MVP notes

- Start with draft-only mode before enabling send mode.
- Keep a strict allowlist for issues the agent can answer autonomously.
- Log retrieval evidence so support leads can audit why a reply was drafted.
