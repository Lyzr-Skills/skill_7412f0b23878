# Persona Analysis Prompt

```markdown
Identify the human actors inside the selected primary ICP.
For each persona, map:
- Role
- Responsibilities
- Goals
- Pain Points (Functional, Financial, Operational, Emotional, Social, Strategic)
- Confidence Level (verified, observed, inferred, hypothesis, unknown, contradictory)

If no source data exists to verify a trait, output:
{
  "value": null,
  "status": "unknown",
  "reason": "insufficient_evidence",
  "evidence_required": [...]
}
Do not hallucinate age range or gender profiles.
```
