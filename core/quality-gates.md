# Quality Gates

To prevent hallucinating generic profile details, the pipeline enforces three mathematical gates:

1. **Evidence Threshold Gate**
   - A persona trait cannot be flagged as `verified` unless mapped to at least 3 distinct first-party customer statement IDs (`EV-xxx`).
   - If 1-2 source references are available, classification is restricted to `observed_signal` or `inferred`.
   - If 0 references, status must be `unknown`.

2. **Confidence Level Gate**
   - Total Segment Confidence score must be >= 70% to trigger primary ICP selection. Otherwise, pipeline returns warning and lists all candidates as hypotheses.

3. **Disconfirming Evidence Gate**
   - Every claim is audited for conflicting evidence. If conflicting signals exist, the confidence score is decayed proportionally by a contradiction penalty formula.
