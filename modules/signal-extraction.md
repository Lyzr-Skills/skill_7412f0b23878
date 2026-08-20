# Signal Extraction Module

Processes raw evidence logs to pull recurring pain points, behaviors, and frequency patterns.

## Output Target
Each signal maps to `customer-signal.json`.
Every signal requires a non-empty `evidence_refs` array indicating which `EV-xxx` source objects contain the raw statement or observation.
