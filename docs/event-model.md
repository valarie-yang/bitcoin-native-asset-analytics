# Event Model

```text
RAW_PROTOCOL_EVENT
  → NORMALIZED_EVENT
      type: DEPLOY | MINT | TRANSFER
      protocol: ORDINALS | BRC20 | RUNES
      txid
      blockHeight
      address
      assetId
      amount / inscriptionRef
  → TRANSACTION_VIEW
  → UTXO / ADDRESS_RELATIONSHIP
  → HOLDING / ASSET_ANALYTICS
```

## Product requirement

Normalization should make protocol-specific activity comparable without pretending the underlying protocols are identical.

## Example product states

- `RAW_RECEIVED`
- `PARSED`
- `NORMALIZED`
- `INDEXED`
- `VALIDATION_EXCEPTION`

A delayed indexer or normalization exception should be visible to internal users so the product does not silently present stale holdings as current.
