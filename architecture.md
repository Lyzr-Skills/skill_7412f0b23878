# Architecture Specification

```mermaid
graph TD
    A[Raw Evidence evidence.json] -->|evidence_refs| B[Customer Signals customer-signal.json]
    B -->|signal_refs| C[Segment Candidates segment.json]
    C -->|segment_refs| D[Segment Comparison & ICP Scoring]
    D -->|Selected Segment| E[ICP Output icp.json]
    E -->|Snapshots| E2[ICP Drift Detection icp-snapshot.json]
    E -->|ICP Match| F[Persona Discovery persona.json]
    F -->|Buying Committee| G[Buying Committee buying-role.json]
    F -->|Pain & Triggers| H[Buying Journey & Triggers]
    F -->|Objections & Channels| I[Messaging & Channels]
    G & H & I --> J[Analysis Report analysis-report.json]
```

## Traceability Path
Every node in the graph relies on a valid parent reference ID. If any link in the chain breaks, the downstream quality gate fails and sets status to `"unknown"`.
- `EV-xxx` -> Raw Evidence
- `SIG-xxx` -> Extracted Customer Signal
- `SEG-xxx` -> Segment Candidates
- `ICP-xxx` -> Target Ideal Customer Profile
- `PER-xxx` -> Discovered Personas
