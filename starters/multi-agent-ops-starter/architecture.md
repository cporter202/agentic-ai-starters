# Architecture

## Core components

- router or planner agent
- specialist worker agents
- reviewer or verifier agent
- orchestration layer for retries and dependencies
- shared memory or task-state store
- trace, metrics, and alerting layer

## Suggested flow

1. Receive a task and classify complexity, risk, and required tools.
2. Break work into bounded subtasks with clear ownership.
3. Execute specialist tasks in parallel where safe.
4. Run a reviewer pass before final delivery or side effects.
5. Store traces, results, and failed-step diagnostics.

## MVP notes

- Start with planner, worker, and reviewer roles before adding more agents.
- Make ownership explicit so agents do not overwrite each other.
- Add timeout, retry, and human-escalation paths early.
