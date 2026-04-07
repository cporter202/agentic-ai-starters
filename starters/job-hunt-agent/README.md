# Job Hunt Agent

Build an assistant that discovers roles, scores fit, tracks applications, and helps candidates move faster with less chaos.

## What it does

This starter monitors job sources, extracts role details, scores openings against a candidate profile, drafts tailored application assets, and keeps the entire funnel organized.

## Who it is for

- job seekers
- career coaches
- recruiting communities
- bootcamps
- executive assistants supporting searches

## Workflow

1. Define role targets, locations, compensation ranges, and exclusions.
2. Pull and normalize job listings.
3. Score each role for fit, urgency, and likely competitiveness.
4. Draft tailored resumes, cover letters, or outreach notes.
5. Track applications, follow-ups, and interview prep tasks.

## Inputs and outputs

Inputs: resume, preferred roles, location, salary targets, industries, constraints.

Outputs: ranked job feed, tailored application assets, follow-up reminders, search dashboard.

## Recommended API stack

- [LinkedIn Jobs Scraper](https://apify.com/valig/linkedin-jobs-scraper?fpr=p2hrc6) for high-signal job discovery
- [Indeed Jobs Scraper](https://apify.com/valig/indeed-jobs-scraper?fpr=p2hrc6) for broader market coverage
- [LinkedIn Company Data Extractor](https://apify.com/data-slayer/linkedin-company-scraper?fpr=p2hrc6) for employer context
- OpenAI and Notion or a tracker database for fit scoring, application assets, and search management

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Job searching is repetitive, fragmented, and emotionally expensive. A strong workflow reduces busywork and creates a clear operating cadence.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
