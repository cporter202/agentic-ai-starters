# Competitor Intel Agent

Build a system that watches competitors and turns their public moves into strategic updates instead of random tabs in a browser.

## What it does

This starter tracks pricing pages, product pages, changelogs, hiring activity, messaging shifts, and web traffic signals, then packages the results into a recurring intel brief.

## Who it is for

- SaaS founders
- product marketers
- strategy teams
- agencies
- B2B operators

## Workflow

1. Define the competitor set and watch surfaces.
2. Capture recurring snapshots of key pages and public signals.
3. Detect meaningful changes in messaging, pricing, feature positioning, and traction proxies.
4. Group changes into narratives and implications.
5. Ship weekly or event-driven competitor briefs.

## Inputs and outputs

Inputs: competitor list, URLs to monitor, watch rules, reporting cadence.

Outputs: change log, positioning summary, pricing deltas, hiring signals, strategy brief.

## Recommended API stack

Use Firecrawl for page snapshots, Similarweb for traffic context, BuiltWith for technology shifts, and OpenAI for interpretation and brief generation.

## Why build it

Good competitor research is expensive to maintain manually, while an autonomous workflow can create compounding strategic context over time.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
