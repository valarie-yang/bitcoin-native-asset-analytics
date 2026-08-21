# Product Decisions

## Normalize before visualizing
Protocol-specific events need a stable object / field model before dashboards can be trusted.

## Asset view vs. address view
Asset discovery answers “what is this asset doing?” while address analytics answers “what does this holder / address own and do?” They should connect but not be collapsed.

## Fact vs. inference
Block / transaction / UTXO facts should remain visually and structurally distinct from risk labels or behavioral inference.

## Coverage vs. data quality
Adding more protocols quickly can create inconsistent semantics. Product scope should prioritize reliable normalization and validation before expanding protocol coverage.
