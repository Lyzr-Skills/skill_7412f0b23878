# Troubleshooting

## Validation Failure
- **Cause**: A downstream conclusion node is missing parent evidence or signal IDs.
- **Fix**: Check `evidence_refs` or `signal_refs` in the target file. Ensure all references exist in the source logs.

## Drift Warning Escalation
- **Cause**: Active customer characteristics differ from stored targets.
- **Fix**: Re-run Stage 5 (Scoring) and select a new primary ICP.
