# Architecture

## Core components

- MCP server registry
- tool-permission and approval layer
- planner and task router
- tool execution runtime
- memory or task-log layer
- observability and replay support

## Suggested flow

1. Receive a user request and classify the needed capabilities.
2. Choose the right tools and ask for approval where required.
3. Execute tool calls step by step with structured reasoning.
4. Save outputs, logs, and follow-up tasks.
5. Return a user-facing result plus an audit trail.

## MVP notes

- Begin with a narrow tool surface and strict approval rules.
- Separate browsing, writing, and action-taking permissions.
- Add replayable traces before expanding into higher-risk automations.
