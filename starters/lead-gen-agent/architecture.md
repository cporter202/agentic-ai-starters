# Architecture

## Core components

- ICP intake form and filter layer
- account discovery engine
- enrichment and verification pipeline
- lead scoring agent
- output adapter for CRM, sheets, or outbound system
- review queue for low-confidence matches

## Suggested flow

1. Convert ICP rules into search queries and filtering logic.
2. Collect account candidates from maps, search, or curated sources.
3. Enrich each record with company, person, and contact data.
4. Score and segment the list by fit and likelihood to respond.
5. Export the best records with reasoning for downstream actions.

## MVP notes

- Keep discovery and enrichment decoupled so you can swap providers later.
- Track confidence separately for business discovery, contact data, and fit scoring.
- Add suppression rules to avoid duplicate outreach or bad-fit industries.
