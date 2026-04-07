# Architecture

## Core components

- market and buy-box intake
- listing and rent-data connectors
- neighborhood enrichment layer
- underwriting and fit-scoring agent
- alerts and operator dashboard
- review queue for top opportunities

## Suggested flow

1. Normalize the acquisition criteria into hard filters and soft preferences.
2. Pull listing, rent, and nearby-place signals on a schedule.
3. Score properties against the buy box and cash-flow logic.
4. Summarize why each shortlisted property stands out.
5. Deliver alerts and review packets to the human operator.

## MVP notes

- Start with one metro and one strategy, such as small multifamily or STR.
- Separate model-generated commentary from hard numeric calculations.
- Keep underwriting formulas inspectable and editable.
