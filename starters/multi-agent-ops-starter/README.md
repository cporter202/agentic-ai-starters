# Multi-Agent Ops Starter

Build a production-style multi-agent workflow with planners, specialists, reviewers, and handoff rules.

## What you are building

This starter is for a system that splits work across multiple agents with clear responsibilities. One agent plans, others execute bounded tasks, and a reviewer checks the result before anything important is released.

The point is not to say "multi-agent" because it sounds advanced. The point is to create specialization, better retries, and safer outputs once a single-agent loop stops being enough.

## Who should build it

- teams building serious agent products
- workflow automation builders
- AI infrastructure operators
- agencies delivering high-touch automations
- founders moving from demo to production

This starter is strongest once you already know a single-agent workflow is too brittle or overloaded.

## End-to-end workflow

1. Route a task to a planner agent.
2. Break the task into specialist subtasks.
3. Send subtasks to worker agents.
4. Run a reviewer pass before final output or risky actions.
5. Retry, escalate, or ship the result.
6. Save traces and summaries for operators.

## Inputs and outputs

Inputs:

- task request
- routing rules
- role definitions
- tool permissions
- quality thresholds

Outputs:

- completed task bundle
- worker outputs
- reviewer notes
- retry queue
- operator summary

## How to build the MVP

Start with three roles only: planner, worker, reviewer. More roles usually add confusion before they add value.

### MVP shape

1. Create a router that classifies the task.
2. Build a planner that outputs:
   subtasks, dependencies, and expected return format.
3. Create one or two worker roles with narrow responsibility.
4. Add a reviewer that checks:
   correctness, completeness, and risk.
5. Save every handoff in a shared task record.
6. Add timeout and retry rules before you add more agent types.

## Core system components

- router
- planner agent
- worker agents
- reviewer agent
- orchestration layer
- task-state store
- trace and metrics layer

## Recommended API stack

- [AI Web Research Agent](https://apify.com/devwithbobby/ai-web-research-agent?fpr=p2hrc6) for dedicated research-worker tasks
- [AI Web Scraper](https://apify.com/apify/ai-web-scraper?fpr=p2hrc6) for flexible extraction-worker tasks
- [Website Content Crawler](https://apify.com/apify/website-content-crawler?fpr=p2hrc6) for knowledge ingestion across agents
- OpenAI, Anthropic, Trigger.dev, and Langfuse for planning, review, orchestration, and observability

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Human checkpoints matter when:

- a task could trigger external side effects
- the planner is uncertain
- workers disagree
- the reviewer flags risk
- retries exceed the safe threshold

## What a strong v1 looks like

A strong v1 should make it obvious:

- which agent owns what
- what each handoff contains
- where failures happen
- when a human should step in

If those answers are unclear, the system is not operationally ready yet.

## Monetization ideas

- multi-agent backends for internal teams
- premium workflow automation systems for agencies
- orchestration products for vertical AI tools
- operator-facing infrastructure for serious AI apps

## Fastest path to v1

1. One planner
2. One worker
3. One reviewer
4. Shared task state
5. Retry and escalation rules

That is enough to create a real multi-agent system without drifting into unnecessary architecture complexity.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

