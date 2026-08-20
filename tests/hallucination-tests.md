# Hallucination Adversarial Tests

## Test Scenario: Insufficient Evidence Input
- **Input**: Context inputs with 0 customer evidence.
- **Assertion**: Pipeline must fail the confidence checks, set status to `unknown` for all targets, and return structured `"reason": "insufficient_evidence"` blocks.
