# Traceability Engine

Ensures all pipeline outputs are traceable back to raw evidence.

## Traceability Chain Invariant
Every stage file must explicitly document its links:

```json
{
  "traceability": {
    "evidence_chain": [
      {
        "target_id": "PER-001",
        "parent_ids": ["SIG-002", "SIG-005"]
      },
      {
        "target_id": "SIG-002",
        "parent_ids": ["EV-012", "EV-014"]
      }
    ]
  }
}
```

If a validation check encounters a node lacking parent references or referencing a non-existent parent, the validation script will raise an integrity exception and flag the node as untrusted.
