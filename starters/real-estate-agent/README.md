# Real Estate Agent

Build a property intelligence workflow that monitors listings, enriches neighborhood context, and helps operators evaluate opportunities faster.

## What it does

This starter pulls listing and rent data, monitors target markets, summarizes nearby amenities and risk factors, and turns raw property information into acquisition or operating insight.

## Who it is for

- real estate investors
- wholesalers
- brokers
- acquisition teams
- property research operators

## Workflow

1. Define markets, buy box, and underwriting assumptions.
2. Collect listings, rent estimates, and neighborhood context.
3. Score properties for fit and investigate notable deltas.
4. Generate operator notes, comps, and follow-up tasks.
5. Route top opportunities to a human review pipeline.

## Inputs and outputs

Inputs: target markets, price range, property type, strategy, rent assumptions.

Outputs: ranked properties, comp notes, market snapshots, underwriting summaries, alert feed.

## Recommended API stack

Use RentCast for listing and rent data, Google Places for amenity and neighborhood signals, OpenAI for underwriting notes and summaries, and Resend or Slack for alert delivery. See [`stack.md`](./stack.md) for the featured Apify picks and tracked direct links.

## Why build it

Real estate workflows benefit from constant monitoring, structured comparison, and fast triage, which makes them a strong fit for autonomous agents with human approval.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
