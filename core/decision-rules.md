# Decision Rules

These rules resolve processing logic inside the pipeline:

1. **Contradictory Evidence Rules**
   - If two first-party source statements directly contradict (e.g., Customer A says "high cost", Customer B says "too cheap"), the system must escalate the issue, split the candidates into sub-segments, and mark the corresponding trait confidence as `contradictory`.
2. **Disqualification Invariants**
   - Any segment score that triggers a disqualifier flag (e.g. Willingness to Pay score < 2) is automatically categorized under the Avoid / Low-fit Segment list.
3. **Drift Alarm Rules**
   - If actual current customers (evidence gathered over last 30 days) score < 60% alignment with stored ICP config, register drift alarm state.
