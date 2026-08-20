# Scoring Adversarial Tests

## Test Scenario: Config Weight Extreme Bounds
- **Input**: Config weights configured to 0.0 or 1.0.
- **Assertion**: Segment scoring equations must prevent divide-by-zero errors and normalize outputs between 0 and 100.
