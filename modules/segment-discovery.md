# Segment Discovery Module

Analyzes patterns in extracted customer signals (`SIG-xxx`) to define candidate targets (e.g. Enterprise SaaS vs mid-market ecommerce). Output targets are saved as `segment.json` candidates.

## Integrity Checks
- Group signals by shared firmographics.
- Reject segment candidate generation if no underlying signals link to it.
