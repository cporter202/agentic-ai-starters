# Customer Support Agent

Build a support workflow that triages tickets, drafts useful replies, and escalates the right issues instead of overwhelming the team.

## What it does

This starter pulls support conversations, classifies intent and urgency, retrieves relevant knowledge, drafts or sends low-risk responses, and routes complex cases to a human support lead.

## Who it is for

- SaaS support teams
- ecommerce operators
- agencies
- customer success teams
- internal ops teams

## Workflow

1. Ingest tickets, chats, or inbox threads.
2. Classify issue type, urgency, and account context.
3. Retrieve the most relevant help-center or internal knowledge.
4. Draft a reply or suggest next steps.
5. Escalate billing, retention, bug, or sensitive issues.

## Inputs and outputs

Inputs: tickets, customer metadata, knowledge-base content, SLAs, escalation rules.

Outputs: triage labels, draft replies, escalation queue, support summaries, resolution insights.

## Recommended API stack

Use Zendesk for ticket workflows, Notion for internal knowledge, Slack for internal escalation, and OpenAI for retrieval-aware drafting and classification. See [`stack.md`](./stack.md) for the featured Apify picks and tracked direct links.

## Why build it

Support teams need speed and consistency, but they also need careful boundaries. This starter is designed to automate the repetitive work without hiding risky decisions.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
