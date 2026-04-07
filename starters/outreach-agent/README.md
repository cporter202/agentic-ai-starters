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

- [Find B2B Emails for Outreach](https://apify.com/purple_beep_boop/find-b2b-emails-for-outreach?fpr=p2hrc6) for outreach-ready contact discovery
- [Linkedin Leads Generator](https://apify.com/contacts-api/linkedin-leads-generator?fpr=p2hrc6) for prospect sourcing
- [LinkedIn Profile Scraper](https://apify.com/automation-lab/linkedin-profile-scraper?fpr=p2hrc6) for personalization context
- OpenAI, Hunter, and Resend for sequence writing, verification, and delivery

See [`stack.md`](./stack.md) for lean, best-value, and premium build paths.

## Why build it

Outbound becomes far more defensible when the workflow combines qualification, personalization, and disciplined operational rules instead of blast-volume automation.

See also: [`architecture.md`](./architecture.md), [`prompts.md`](./prompts.md), [`stack.md`](./stack.md)
