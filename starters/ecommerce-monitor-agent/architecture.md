# Architecture

## Core components

- source connectors for store, marketplace, and competitor data
- normalization pipeline for SKUs, prices, reviews, and availability
- change-detection service
- summarization and action-recommendation agent
- alerting and reporting outputs
- review layer for major pricing or stock anomalies

## Suggested flow

1. Pull product data from owned and observed sources.
2. Normalize product entities across channels.
3. Detect deltas in price, stock, rating, or assortment.
4. Generate change summaries with likely impact and urgency.
5. Send alerts or dashboards to operators.

## MVP notes

- Start with one catalog segment and a small competitor set.
- Use change windows to avoid duplicate noisy alerts.
- Track entity matching carefully when competitor product names are inconsistent.
