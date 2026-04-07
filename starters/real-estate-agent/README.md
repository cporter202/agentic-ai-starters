# Real Estate Agent

Build a property intelligence workflow that monitors listings, enriches neighborhood context, and helps operators evaluate opportunities faster.

## What you are building

This starter is for a system that watches listings, rent signals, local context, and relevant market details, then turns that information into shortlists and operator notes.

The right version of this product feels like a sourcing and screening assistant for investors, operators, or acquisition teams.

## Who should build it

- real estate investors
- wholesalers
- brokers
- acquisition teams
- property research operators

This starter is strongest when users have a defined buy box and need help screening opportunities at scale.

## End-to-end workflow

1. Define target markets and acquisition criteria.
2. Pull listing and rent data on a schedule.
3. Add neighborhood and amenity context.
4. Score properties against the buy box.
5. Draft short investment notes or follow-up packets.
6. Route shortlisted properties for manual review.

## Inputs and outputs

Inputs:

- target markets
- price range
- property type
- strategy such as rental, flip, or long-term hold
- buy-box rules
- alert thresholds

Outputs:

- ranked listing feed
- screening notes
- market and amenity context
- underwriting summary
- shortlist alerts

## How to build the MVP

Start with one geography and one strategy. That is the easiest way to make the scoring logic trustworthy.

### MVP shape

1. Build a market configuration layer for:
   city, neighborhoods, property type, and price range.
2. Pull listing data and structured property fields.
3. Add rent and nearby context.
4. Score each property by:
   match quality, upside, missing data, and attention priority.
5. Draft a short note that explains:
   why it made the shortlist and what to verify next.
6. Send a human review packet rather than trying to automate the final acquisition decision.

## Core system components

- buy-box intake
- listing collector
- market enrichment layer
- screening and underwriting layer
- shortlist generator
- review workflow

## Recommended API stack

- [Zillow Scraper](https://apify.com/mido_99/zillow-scraper?fpr=p2hrc6) for listing intelligence
- [Google Maps B2B Leads Scraper](https://apify.com/primeparse/google-maps-scraper?fpr=p2hrc6) for location and nearby-business context
- [Google Search API](https://apify.com/api/google-search-api?fpr=p2hrc6) for market and locality discovery
- RentCast, OpenAI, and Resend or Slack for underwriting notes, structured property data, and alerts

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Always keep manual review for:

- financial assumptions
- title or legal issues
- unusual listings
- missing rent or property data
- any purchase or offer decision

## What a strong v1 looks like

A strong v1 helps the operator answer:

- does this fit the buy box?
- what is missing?
- why is this interesting?
- what should I verify next?

That is enough to create real value before you build full underwriting software.

## Monetization ideas

- investor deal-sourcing tools
- acquisition-assistant products
- research services for small teams
- local market watch products for niche operators

## Fastest path to v1

1. One market
2. One strategy
3. Listing pull
4. Screening logic
5. Human shortlist review

That gets you to a useful sourcing workflow much faster than trying to automate the whole investment stack.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
