# Evidence Adversarial Tests

## Test Scenario: Contradictory Logs
- **Input**: Equal numbers of high-weight positive and negative customer statements.
- **Assertion**: Classification must yield `"contradictory"` status and decay downstream pipeline confidence scores.
