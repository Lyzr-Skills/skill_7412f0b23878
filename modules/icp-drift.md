# ICP Drift Detection Module

Compares current active customer traits derived from the latest evidence entries against the stored target baseline `icp.json`.

## Drift Calculation
- If the divergence score exceeds 25% (e.g. active users are predominantly early-stage startups while stored ICP is mid-market SaaS), trigger drift warning state.
- Save run results as a snapshot in `icp-snapshot.json`.
