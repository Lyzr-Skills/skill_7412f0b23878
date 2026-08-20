# Workflow Specification

## Phase 1 — Define Business Context
- Collect and analyze business invariants (company profile, geography, sales model, etc.).
- Output standard context map.

## Phase 2 — Evidence Collection
- Load and parse transcripts, reviews, CRM records, and external conversations.
- Assign structured `EV-xxx` identifiers.

## Phase 3 — Signal Extraction
- Extract objective facts, customer quotes, and observations from raw evidence.
- Map to `SIG-xxx` referencing parent `EV-xxx` identifiers.

## Phase 4 — Segment Discovery
- Generate Candidate Segments based on observed patterns.
- Map to `SEG-xxx` referencing parent `SIG-xxx` identifiers.

## Phase 5 — ICP Scoring & Segment Comparison
- Run segment evaluations on the 10-dimension model using configurable weights.
- Compare scores side-by-side. Highlight relative win/loss drivers.

## Phase 6 — ICP Selection & Drift Verification
- Target primary segment and document secondary and negative/disqualified segments.
- Check against historic snapshots to flag profile drift.

## Phase 7 — Persona & Buying Committee Discovery
- Discover the human decision makers in the B2B context (User, Champion, Buyer, Blocker).
- Link back to evidence.

## Phase 8 — Pain & Purchase Trigger Analysis
- Document functional, operational, financial, emotional, and social pains.
- Identify the internal, external, or event-based purchase triggers.

## Phase 9 — Journey, Objection & Channel Analysis
- Match buying committee roles to buying stages.
- Map objections (trust, price, complexity) and preferred information channels.

## Phase 10 — Messaging & Executive Report Generation
- Construct pain-point specific messaging hooks.
- Generate final analysis report referencing evidence chains.
