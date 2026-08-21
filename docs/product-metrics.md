# Proposed Product Metrics

These are portfolio metrics, not claimed historical production results.

## Data coverage & quality
- protocol / event-type coverage
- normalization exception rate
- missing / duplicate event rate
- indexer freshness / delay

## Product usage
- search success / zero-result rate
- asset-page completion
- address-analysis completion
- drill-down rate from alert → entity → transaction evidence

## Monitoring quality
- alert review rate
- dismissal rate
- time to review
- label precision where reviewed ground truth exists

## Product principle
Metrics should distinguish data-pipeline quality from user behavior. A low page-conversion rate and stale indexing are different problems and require different owners.
