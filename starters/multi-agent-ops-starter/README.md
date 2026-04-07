# Multi-Agent Ops Starter

Build a production-style multi-agent workflow with planners, specialists, reviewers, and handoff rules.

## What it does

This starter gives you a blueprint for orchestrating multiple agents that split research, execution, verification, and reporting across a shared workflow with observability and human checkpoints.

## Who it is for

- teams building serious agent products
- workflow automation builders
- AI infrastructure operators
- agencies delivering high-touch automations
- founders moving from demo to production

## Workflow

1. Route a task to a planner agent.
2. Decompose the work into specialist subtasks.
3. Let worker agents gather data or execute steps.
4. Run a reviewer agent before any risky or final output.
5. Publish results and trace logs to operators.

## Inputs and outputs

Inputs: task request, routing rules, model policy, tool permissions, SLAs.

Outputs: completed task bundle, trace data, reviewer notes, retry queue, operator summary.

## Recommended API stack

Use OpenAI for the planner or executor roles, Anthropic for review or long-context specialists, Trigger.dev for reliable orchestration, Langfuse for traces, and Slack for human checkpoints.

## Why build it

Many autonomous applications outgrow a single-agent loop quickly. Multi-agent patterns help once you need specialization, review, retries, and operational visibility.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
