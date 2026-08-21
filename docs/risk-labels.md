# Risk Labels & Monitoring

Public-safe product categories represented in the portfolio case include:

- suspicious assets
- suspicious addresses
- abnormal transfers
- price / activity anomalies
- high-frequency activity

These are product monitoring labels. Unless a formal compliance rule set exists, they should not be presented as legal or compliance determinations.

## Recommended fields

- `labelType`
- `entityType`
- `entityId`
- `ruleVersion`
- `evidenceRefs[]`
- `severity`
- `status`
- `reviewedBy`
- `reviewedAt`

## Review states

```text
DETECTED → QUEUED → UNDER_REVIEW → CONFIRMED / DISMISSED
```

The product should preserve the evidence and rule version that produced the label so future reviewers can understand why it appeared.
