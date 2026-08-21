# Data Model

| Object | Product purpose | Example fields |
|---|---|---|
| Token / Inscription | Protocol-specific asset identity and metadata | protocol, assetId, ticker, inscriptionId, deployTx |
| UTXO | Bitcoin-native location / spend state relevant to assets | txid, vout, value, spentStatus, inscriptionRef |
| Address | Holdings and activity aggregation | address, firstSeen, lastActive, labelStatus |
| Holding | User-facing ownership state | address, assetId, balance, asOf |
| Transaction | On-chain movement | txid, blockHeight, timestamp, status |
| Event | Deploy / Mint / Transfer semantics | eventType, assetId, address, amount, txid |
| Risk Label | Monitoring / inference separated from chain facts | labelType, severity, evidenceRefs, status |

## Product principle

The analytics layer should keep raw chain facts, normalized product objects and inferred monitoring labels structurally distinct. This makes the UI easier to explain and reduces the risk of presenting an inference as a protocol fact.
