# MCP Toolchain Starter

Build an MCP-first agent that can use real tools, docs, repos, workspaces, and operator systems instead of living inside a pure chat loop.

## What you are building

This starter is for a tool-using agent system. It should receive a request, choose the right tools, operate with clear permissions, and return a result with an audit trail.

The value here is not "chat with tools." The value is reliable task execution across real systems with guardrails.

## Who should build it

- AI product teams
- internal tooling teams
- founders building agent workflows
- developer experience teams
- consultants building custom copilots

This starter is strongest when the product needs to touch docs, repos, workspaces, support systems, or internal knowledge safely.

## End-to-end workflow

1. Accept a user request and identify the required capabilities.
2. Choose the minimum tool surface needed.
3. Ask for approval where required.
4. Execute tool calls in a controlled order.
5. Save outputs, logs, and follow-up tasks.
6. Return a result and a clear activity trail.

## Inputs and outputs

Inputs:

- user request
- tool registry
- permission rules
- approval policy
- workspace scope

Outputs:

- completed task result
- action log
- notes or artifacts
- follow-up tasks
- review-ready trace

## How to build the MVP

Keep the first version narrow. One useful agent with a small, safe tool surface beats a huge tool graph with weak controls.

### MVP shape

1. Define three to five allowed tools.
2. Create a router that maps requests to tool groups.
3. Add approval logic for:
   write actions, destructive actions, or external side effects.
4. Add a structured execution loop:
   plan, call tool, inspect output, continue or stop.
5. Save a trace of:
   tool choice, tool output, final result, and failures.
6. Add replay and debugging before you add more tools.

## Core system components

- tool registry
- router and planner
- permission layer
- tool execution runtime
- trace store
- approval and review workflow

## Recommended API stack

- [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) for structured web actions
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for docs and knowledge ingestion
- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for live web retrieval
- OpenAI, GitHub, Notion, and Slack for tool-aware reasoning, repo actions, docs, and approvals

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Add approval or review for:

- deletes and edits
- outbound communications
- repo or production changes
- low-confidence tool choices
- repeated failure loops

## What a strong v1 looks like

A strong v1 should make it easy to answer:

- what did the agent do?
- which tools did it use?
- what side effects occurred?
- can I replay or audit this later?

Those questions matter more than surface-level cleverness.

## Monetization ideas

- internal copilots for teams
- agent platforms for consulting clients
- MCP-based workflow products
- operator assistants for support, sales, or engineering

## Fastest path to v1

1. Small tool registry
2. Router
3. Permission rules
4. Execution trace
5. Human approval for risky actions

That gives you a trustworthy tool-using agent much faster than trying to launch a general-purpose operator from day one.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

