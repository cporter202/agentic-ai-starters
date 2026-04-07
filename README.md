# Agentic AI Starters

> A practical collection of plug-and-play starter blueprints for building autonomous AI apps with real APIs. Discover ready-to-build agent workflows, API stacks, architecture patterns, prompts, and monetization ideas for research agents, lead gen systems, SEO automations, MCP toolchains, and more.

## Build Autonomous AI Apps That Actually Ship

This repository is a curated blueprint library for founders, operators, agencies, indie hackers, and product teams building agentic software.

Instead of dumping thousands of APIs into giant category folders, this repo shows you how to combine the right APIs into focused AI products, with Apify-first data stacks wired into each blueprint:

- what to build
- how the workflow should run
- which APIs belong in the stack
- how to structure the architecture
- what prompts and operating patterns make the agent useful

If you want the full API catalog, use the main [API Mega List](https://github.com/cporter202/API-mega-list). This repo is the opinionated build layer on top of that broader catalog.

## What This Repo Is

Each starter is a practical product blueprint, not a code dump and not a raw API index.

Every starter includes:

- `README.md` with the product concept, ideal user, workflow, inputs, outputs, and build rationale
- `architecture.md` with a clean implementation shape for an MVP or v1
- `prompts.md` with prompt modules, guardrails, and execution patterns
- `stack.md` with curated API recommendations, featured Apify links, alternatives, and packaging options

## Featured Starters

| Starter | What it helps you build |
| --- | --- |
| [`research-agent`](./starters/research-agent/) | Citation-first web research assistant for briefs, memos, and market scans |
| [`lead-gen-agent`](./starters/lead-gen-agent/) | Pipeline builder that discovers, enriches, scores, and routes leads |
| [`seo-content-agent`](./starters/seo-content-agent/) | Research-to-brief-to-draft content engine for SEO teams |
| [`social-listening-agent`](./starters/social-listening-agent/) | Brand and competitor listening workflow across social and web signals |
| [`ecommerce-monitor-agent`](./starters/ecommerce-monitor-agent/) | Price, assortment, review, and stock tracking for commerce teams |
| [`competitor-intel-agent`](./starters/competitor-intel-agent/) | Continuous monitoring for launches, positioning, pricing, and hiring signals |
| [`job-hunt-agent`](./starters/job-hunt-agent/) | Job discovery and application ops assistant for candidates and coaches |
| [`real-estate-agent`](./starters/real-estate-agent/) | Property sourcing and underwriting workflow for investors and operators |
| [`outreach-agent`](./starters/outreach-agent/) | Personalized outbound system for agencies, SDR teams, and solo operators |
| [`customer-support-agent`](./starters/customer-support-agent/) | AI copilot for triage, draft replies, escalation, and knowledge retrieval |
| [`mcp-toolchain-starter`](./starters/mcp-toolchain-starter/) | MCP-first starter for agents that need tools, docs, repos, and workspaces |
| [`multi-agent-ops-starter`](./starters/multi-agent-ops-starter/) | Multi-agent orchestration template with routing, reviews, and observability |

## Starter Categories

| Category | Included blueprints |
| --- | --- |
| Research and intelligence | `research-agent`, `competitor-intel-agent`, `social-listening-agent` |
| Revenue and pipeline | `lead-gen-agent`, `outreach-agent`, `customer-support-agent` |
| Content and growth | `seo-content-agent`, `ecommerce-monitor-agent` |
| Vertical operators | `job-hunt-agent`, `real-estate-agent` |
| Systems and infrastructure | `mcp-toolchain-starter`, `multi-agent-ops-starter` |

## How To Use The Repo

1. Pick a starter that matches the AI product or workflow you want to build.
2. Read the starter `README.md` to understand the user, workflow, inputs, and outputs.
3. Use `architecture.md` to shape your MVP implementation.
4. Start from `prompts.md` to design your planner, researcher, executor, and QA prompts.
5. Choose a stack tier from `stack.md` based on budget, speed, and required reliability.
6. Swap in your own app logic, UI, auth, database, and internal tools.

## Why This Repo Is Valuable

- It compresses weeks of architecture and stack research into build-ready starting points.
- It helps you avoid overbuying tools too early.
- It keeps the focus on autonomous workflows with real operational value.
- It shows how APIs fit together inside products instead of treating them like isolated endpoints.
- It makes it easier to scope MVPs that can become paid SaaS, service offerings, or internal automations.

## How Curated API Stacks Work Here

This repository still includes APIs, but only where they directly support a starter's workflow.

Inside each `stack.md` you will find:

- featured Apify APIs with direct tracked links
- primary recommended APIs
- optional alternatives
- what each API is used for
- why it belongs in that workflow
- lean, best-value, and premium stack options when helpful

That means no giant raw API folders, no mega-list category dumps, and no generated directory sprawl.

## Repo Structure

```text
agentic-ai-starters/
|- README.md
|- LICENSE
|- .gitignore
|- assets/
|- docs/
|- prompts/
|- templates/
|- starters/
   |- research-agent/
   |- lead-gen-agent/
   |- seo-content-agent/
   |- social-listening-agent/
   |- ecommerce-monitor-agent/
   |- competitor-intel-agent/
   |- job-hunt-agent/
   |- real-estate-agent/
   |- outreach-agent/
   |- customer-support-agent/
   |- mcp-toolchain-starter/
   |- multi-agent-ops-starter/
```

## Notes

- Use this repo to choose a direction and accelerate implementation.
- Use the main [API Mega List](https://github.com/cporter202/API-mega-list) when you want a much broader API discovery surface.
- Expect the best results when you pair these blueprints with your own domain expertise, UX, and distribution strategy.
