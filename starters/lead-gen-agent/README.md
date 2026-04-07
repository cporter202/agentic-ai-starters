# Lead Gen Agent

Build an autonomous lead generation workflow that finds accounts, enriches contacts, scores fit, and delivers outreach-ready records.

## What you are building

This starter is for a system that turns an ideal customer profile into a repeatable prospecting machine. It should discover businesses or people, enrich them with useful context, verify contact paths, score them for fit, and push the best records into a CRM, sheet, or outbound queue.

The core idea is simple: stop shipping raw scraped lists and start shipping qualified pipeline inputs.

## Who should build it

- agencies
- SDR teams
- founders
- consultants
- local service operators

This starter is strongest when the user already has a clear offer, target market, and reason for outreach.

## End-to-end workflow

1. Define the ICP, territory, vertical, and exclusion rules.
2. Generate discovery queries based on the ICP.
3. Collect account or person candidates from public sources.
4. Enrich records with company, role, and contact details.
5. Score records for fit, urgency, and completeness.
6. Remove duplicates and low-confidence leads.
7. Export qualified leads for CRM, outbound, or manual review.

## Inputs and outputs

Inputs:

- ICP definition
- industries and geographies
- company-size bands
- keywords and intent signals
- exclusions and suppression rules

Outputs:

- ranked lead list
- contact profiles
- qualification notes
- enrichment fields
- confidence score
- outreach-ready queue

## How to build the MVP

The best first version is not "scrape every source on the internet." It is one reliable lead source plus one enrichment path plus one scoring layer.

### MVP shape

1. Build an ICP intake form that captures:
   niche, location, company type, buyer role, and exclusions.
2. Create a discovery step that returns:
   business or contact candidates with source URLs.
3. Add enrichment for:
   website, company profile, role, and verified contact information.
4. Create a scoring prompt that labels each record:
   strong fit, possible fit, weak fit, or discard.
5. Add duplicate suppression by:
   domain, company name, and email.
6. Export the top records into a sheet or CRM with reasons attached.

## Core system components

- ICP intake form
- discovery engine
- enrichment pipeline
- verification layer
- lead scoring agent
- suppression and dedupe rules
- export adapter for CRM or sheets

## Recommended API stack

- [Linkedin Leads Generator](https://apify.com/contacts-api/linkedin-leads-generator?fpr=p2hrc6) for sourcing prospects
- [Google Maps B2B Leads Scraper](https://apify.com/primeparse/google-maps-scraper?fpr=p2hrc6) for local business discovery
- [LinkedIn Company Data Extractor](https://apify.com/data-slayer/linkedin-company-scraper?fpr=p2hrc6) for company enrichment
- OpenAI, Hunter, and People Data Labs for scoring, verification, and enrichment logic

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Keep people in the loop for:

- weak or partial contact data
- suspicious domains or generic emails
- duplicate companies from multiple sources
- borderline ICP matches
- regulated or sensitive target segments

## What a strong v1 looks like

A strong v1 should reliably answer:

- is this company a fit?
- who should I reach out to?
- do I have enough data to act?
- why did this lead make the final list?

If the user cannot answer those questions from the exported row alone, the product still needs work.

## Monetization ideas

- monthly lead list subscriptions for niche agencies
- prospecting-as-a-service offers
- local lead-gen systems for home services or B2B operators
- outbound enablement tools layered on top of the lead pipeline

## Fastest path to v1

1. One niche
2. One source of discovery
3. One enrichment pass
4. One score
5. One export destination

That is enough to get usable results and user feedback before you add more sources and complexity.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)

