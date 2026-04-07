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

- [Linkedin Leads Generator](https://apify.com/contacts-api/linkedin-leads-generator?fpr=p2hrc6) for sourcing prospects
- [Google Maps B2B Leads Scraper](https://apify.com/primeparse/google-maps-scraper?fpr=p2hrc6) for local business discovery
- [LinkedIn Company Data Extractor](https://apify.com/data-slayer/linkedin-company-scraper?fpr=p2hrc6) for company enrichment
- OpenAI, Hunter, and People Data Labs for scoring, verification, and enrichment logic

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Lead generation has clear ROI, short feedback loops, and plenty of room for vertical specialization by geography, niche, or account type.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
