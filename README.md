# Bitcoin-native Asset Analytics

A product case study for normalizing and analyzing Bitcoin-native assets across Ordinals, BRC-20 and Runes.

**Role lens:** Product Management  
**Focus:** On-chain Data · UTXO · Address Analytics · Event Modeling · Risk Labels

**Portfolio:** [Valarie Yang — Product Portfolio](https://www.figma.com/design/pIUP2RYiUR3fpGoKHjRGnU/Valarie-Yang-%E2%80%94-Product-Portfolio?node-id=0-1)  
**Profile:** [LinkedIn](https://www.linkedin.com/in/valarie-yang-08573b122/) · [GitHub](https://github.com/valarie-yang)

> This public portfolio reconstruction uses synthetic / public-safe examples. It contains no confidential company data and does not claim Bitcoin protocol-core, indexer-engine or compliance ownership.

## My role and scope

- Asset identification, holdings and transaction tracking
- Product object / field definitions
- Deploy / Mint / Transfer event semantics
- Asset, address and transaction analytics surfaces
- Risk labels, monitoring and alerting logic

## Core model

```text
Protocol event
   ↓
Normalize Deploy / Mint / Transfer
   ↓
Transaction
   ↓
UTXO + Address relationships
   ↓
Holding / Asset view
   ↓
Analytics + Monitoring
```

## Key product decisions

1. **Normalize before visualizing** — protocol-specific events need a stable object and field model before dashboards can be trusted.
2. **Separate asset and address jobs** — asset discovery and address behavior analysis should connect without collapsing into one view.
3. **Separate fact from inference** — chain facts remain distinct from risk labels and monitoring categories.
4. **Make data quality visible** — missing / delayed / inconsistent indexing states should be treated as product states, not hidden implementation details.

## Implementation boundary

This case does **not** claim ownership of Bitcoin protocol development, indexer-engine implementation, compliance determinations, exchange pricing infrastructure or smart-contract engineering.

## Repository map

- [`docs/data-model.md`](docs/data-model.md) — core product objects
- [`docs/event-model.md`](docs/event-model.md) — Deploy / Mint / Transfer normalization
- [`docs/risk-labels.md`](docs/risk-labels.md) — monitoring labels and review boundaries
- [`docs/product-decisions.md`](docs/product-decisions.md) — key PM trade-offs
- [`docs/product-metrics.md`](docs/product-metrics.md) — proposed product metrics
- [`data/sample_events.csv`](data/sample_events.csv) — synthetic event sample

## Portfolio connection

This repository supports on-chain data, wallet asset, Web3 analytics, risk-monitoring and exchange asset-product roles. The visual case study is maintained separately in Figma.
