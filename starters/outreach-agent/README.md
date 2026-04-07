# Outreach Agent

Build a personalized outbound system that turns qualified leads into messages, sequences, and follow-up actions.

## What you are building

This starter is for a workflow that takes a lead list, researches the account and contact, drafts relevant outbound messaging, sequences follow-ups, and routes replies or edge cases to a human operator.

The product should help users send fewer, better messages. The point is not spam volume. The point is high-context outbound that creates pipeline.

## Who should build it

- agencies
- founders
- SDR teams
- recruiters
- service businesses

This starter is strongest when the user has a clear offer, case studies, and a narrow target segment.

## End-to-end workflow

1. Accept a lead list or connect to a lead source.
2. Collect company and contact context.
3. Generate personalization angles tied to the offer.
4. Draft first-touch and follow-up messages.
5. Schedule the sequence with stop rules.
6. Classify replies and route them for human action.

## Inputs and outputs

Inputs:

- lead list
- offer
- ICP
- case studies or proof points
- sending rules
- tone and compliance constraints

Outputs:

- personalization notes
- first-touch message
- follow-up sequence
- reply labels
- handoff queue

## How to build the MVP

The smartest first version is one list source, one message channel, and one reply classifier.

### MVP shape

1. Import leads from a CSV, sheet, or upstream lead workflow.
2. Pull enough context to answer:
   why this account, why this person, why now.
3. Generate a short first-touch message and two follow-ups.
4. Add stop conditions for:
   replies, bounces, and suppression.
5. Add a reply classifier for:
   interested, objection, not now, unsubscribe, or wrong person.
6. Route positive replies to a human closer.

## Core system components

- lead intake and suppression rules
- personalization context collector
- message-generation agent
- sequence scheduler
- reply classifier
- human handoff queue

## Recommended API stack

- [Find B2B Emails for Outreach](https://apify.com/purple_beep_boop/find-b2b-emails-for-outreach?fpr=p2hrc6) for outreach-ready contact discovery
- [Linkedin Leads Generator](https://apify.com/contacts-api/linkedin-leads-generator?fpr=p2hrc6) for prospect sourcing
- [LinkedIn Profile Scraper](https://apify.com/automation-lab/linkedin-profile-scraper?fpr=p2hrc6) for personalization context
- OpenAI, Hunter, and Resend for sequence writing, verification, and delivery

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Human review points

Require human review for:

- high-value accounts
- compliance-sensitive segments
- negative or nuanced replies
- claims that depend on customer-specific promises
- unsubscribe and reputation issues

## What a strong v1 looks like

A strong v1 should produce messages that make a human say:

- this feels relevant
- this is short enough
- this is safe to send
- this gives me a clear next step if someone replies

If the output feels generic, the personalization layer is probably too weak.

## Monetization ideas

- outbound systems for niche agencies
- founder-led pipeline assistants
- recruiter outreach tools
- productized outbound setup services

## Fastest path to v1

1. One niche
2. One lead source
3. One message channel
4. One sequence
5. One reply classifier

That path gives you a working outbound product before you expand into full CRM automation.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
