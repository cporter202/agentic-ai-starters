# Customer Support Agent

Build a support workflow that triages tickets, drafts useful replies, and escalates the right issues instead of overwhelming the team.

## What you are building

This starter is for a support system that ingests tickets or messages, classifies the issue, retrieves the right knowledge, drafts a response, and decides whether the conversation is safe for automation or should be handed to a human.

The product should improve support speed and consistency without hiding risky decisions.

## Who should build it

- SaaS support teams
- ecommerce operators
- agencies
- customer success teams
- internal ops teams

This starter is strongest when the team has a repeatable support process and a usable knowledge base, even if that knowledge base is messy.

## End-to-end workflow

1. Ingest tickets, chats, or inbox threads.
2. Classify the issue type, urgency, and sentiment.
3. Retrieve relevant knowledge or prior solved cases.
4. Draft the best next response.
5. Escalate sensitive or high-risk issues.
6. Save resolution data for reporting and workflow improvement.

## Inputs and outputs

Inputs:

- support tickets
- customer metadata
- knowledge-base content
- SLA rules
- escalation rules

Outputs:

- ticket labels
- response drafts
- escalation queue
- support summaries
- resolution insights

## How to build the MVP

Start in draft mode. Do not let the system auto-send on day one.

### MVP shape

1. Connect one support channel such as Zendesk.
2. Normalize every ticket into:
   customer, issue type, urgency, text, and account context.
3. Add a classification step for:
   billing, bug, setup, feature request, refund, or account issue.
4. Add retrieval from help-center and internal docs.
5. Draft a short response using only retrieved knowledge.
6. Route high-risk issues to a human queue.
7. Track acceptance and edit rates so you can improve prompts safely.

## Core system components

- ticket intake
- classification layer
- retrieval layer
- reply-generation agent
- escalation rules
- reporting and analytics layer

## Recommended API stack

- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for help-center and docs ingestion
- [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) for extracting structured support content
- [Trustpilot Scraper](https://apify.com/happitap/trustpilot-scraper?fpr=p2hrc6) for external customer feedback
- Zendesk, Slack, and OpenAI for ticket workflows, escalations, and retrieval-aware drafting

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Always keep humans involved for:

- billing and refund issues
- abusive or legal complaints
- account-specific actions
- retention or cancellation conversations
- low-confidence retrieval matches

## What a strong v1 looks like

A strong v1 does not need full automation. It needs:

- accurate triage
- fast retrieval
- good draft quality
- safe escalation behavior

If the team still has to rewrite most drafts from scratch, the workflow is not ready for scale.

## Monetization ideas

- internal support copilots for SaaS teams
- support automation packages for agencies
- vertical support systems for niche ecommerce stores
- hybrid support tools for small teams without large CX budgets

## Fastest path to v1

1. Ticket ingestion
2. Classification
3. Retrieval
4. Draft generation
5. Human approval

That gives you a real support assistant before you take on auto-send risk.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
