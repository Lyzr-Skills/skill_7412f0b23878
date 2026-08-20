# Persona Discovery Module

Extracts human actors within the selected Primary ICP who interact with the buying decision.

## Invariant Rules
- Every persona candidate must map to at least one `SIG-xxx` reference.
- Demographics or personal habits cannot be generated without active evidence mappings.
- Mapped attributes without evidence are assigned a status of `"unknown"`.
