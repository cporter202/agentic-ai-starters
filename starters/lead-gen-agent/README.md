# Lead Gen Agent

Build an autonomous lead generation workflow that finds accounts, enriches contacts, scores fit, and delivers outreach-ready records.

## What it does

This starter turns an ideal customer profile into a repeatable prospecting system. It discovers businesses or people, enriches key attributes, verifies contact paths, and outputs ranked leads for CRM or outbound use.

## Who it is for

- agencies
- SDR teams
- founders
- consultants
- local service operators

## Workflow

1. Define the ICP, territory, and exclusion rules.
2. Discover accounts from search, maps, or public web signals.
3. Enrich companies and people with firmographic and contact data.
4. Score leads by fit, urgency, and data completeness.
5. Push top leads into a sheet, CRM, or outbound queue.

## Inputs and outputs

Inputs: ICP, industries, geographies, company size, keywords, exclusions.

Outputs: ranked lead list, contact profiles, enrichment fields, qualification notes, follow-up queue.

## Recommended API stack

Use People Data Labs for enrichment, Hunter for email discovery and verification, Google Places or Apify for discovery, and OpenAI for lead scoring and routing logic.

## Why build it

Lead generation has clear ROI, short feedback loops, and plenty of room for vertical specialization by geography, niche, or account type.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
