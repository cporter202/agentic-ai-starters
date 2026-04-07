# Outreach Agent

Build a personalized outbound system that turns qualified leads into messages, sequences, and follow-up actions.

## What it does

This starter takes a lead list, researches the account and contact, drafts personalized messaging, schedules a sequence, and hands off replies or exceptions to a human operator.

## Who it is for

- agencies
- founders
- SDR teams
- recruiters
- service businesses

## Workflow

1. Import leads from a CRM, sheet, or lead-gen pipeline.
2. Research the company, role, and likely pain points.
3. Draft personalized email or DM copy.
4. Sequence follow-ups with stop rules.
5. Route replies, objections, or edge cases to a human.

## Inputs and outputs

Inputs: lead list, offer, ICP, case studies, tone rules, sending domain.

Outputs: message variants, sequence steps, personalization notes, handoff queue, reply labels.

## Recommended API stack

Use People Data Labs or your lead source for enrichment, Hunter for deliverability-aware contact work, Resend for delivery, and OpenAI for personalization and objection handling. See [`stack.md`](./stack.md) for the featured Apify picks and tracked direct links.

## Why build it

Outbound becomes far more defensible when the workflow combines qualification, personalization, and disciplined operational rules instead of blast-volume automation.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
