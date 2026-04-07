# Job Hunt Agent

Build an assistant that discovers roles, scores fit, tracks applications, and helps candidates move faster with less chaos.

## What you are building

This starter is for a workflow that monitors job listings, enriches company context, scores role fit, drafts tailored application assets, and keeps the search organized from first discovery to follow-up.

The strongest version of this product behaves like a job-search operating system, not just a job board wrapper.

## Who should build it

- job seekers
- career coaches
- recruiting communities
- bootcamps
- executive assistants supporting searches

This starter works best when users need structure, prioritization, and faster tailoring rather than just more listings.

## End-to-end workflow

1. Define target roles, compensation, location, and exclusions.
2. Pull and normalize job listings.
3. Score listings for fit and priority.
4. Enrich employer context.
5. Draft tailored resume summaries, cover letters, or outreach notes.
6. Track applications, interviews, and follow-up tasks.

## Inputs and outputs

Inputs:

- resume or profile
- preferred roles
- location rules
- salary targets
- industry preferences
- exclusions

Outputs:

- ranked job feed
- fit score
- application assets
- follow-up reminders
- interview prep queue

## How to build the MVP

Start with one role family such as SDR, product manager, designer, or engineer. Fit scoring becomes much better when the target is narrow.

### MVP shape

1. Accept a candidate profile and constraints.
2. Pull listings from one or two sources.
3. Normalize jobs into one schema:
   title, company, location, salary, URL, and requirements.
4. Score the listing against:
   skills, seniority, location, and upside.
5. Generate a short candidate-specific rationale for the top matches.
6. Add draft generation for application assets only after scoring works well.
7. Track status changes in a simple board or database.

## Core system components

- candidate profile intake
- listing collector
- normalization and dedupe layer
- fit-scoring agent
- asset generator
- application tracker

## Recommended API stack

- [LinkedIn Jobs Scraper](https://apify.com/valig/linkedin-jobs-scraper?fpr=p2hrc6) for high-signal job discovery
- [Indeed Jobs Scraper](https://apify.com/valig/indeed-jobs-scraper?fpr=p2hrc6) for broader market coverage
- [LinkedIn Company Data Extractor](https://apify.com/data-slayer/linkedin-company-scraper?fpr=p2hrc6) for employer context
- OpenAI and Notion or a tracker database for fit scoring, application assets, and search management

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Keep human control for:

- final application submissions
- resume edits
- cover letter tone
- interview strategy
- claims about candidate experience

## What a strong v1 looks like

A strong v1 helps the user answer:

- which jobs are actually worth applying to?
- why is this a fit?
- what should I send?
- what do I need to follow up on today?

That is more useful than just aggregating listings.

## Monetization ideas

- job-search assistants for candidates
- cohort tools for bootcamps
- career-coach workflow products
- premium job-match and application packages

## Fastest path to v1

1. One role family
2. One or two listing sources
3. Fit scoring
4. Tailored application draft
5. Pipeline tracking

That gets you to a valuable search workflow without overbuilding a career platform.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
