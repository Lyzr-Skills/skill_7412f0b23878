# Confidence Model

Mathematical formula to calculate trait confidence:

\[ C_{trait} = \frac{\sum (W_{source} \times R_{score})}{N} \times (1 - P_{contradiction}) \]

Where:
- \(W_{source}\) = Weight of the source (1.0 first-party, 0.7 external, 0.3 synthetic).
- \(R_{score}\) = Recency factor (1.0 for <= 90 days, decaying to 0.1 for > 365 days).
- \(P_{contradiction}\) = Contradiction penalty (0.0 to 1.0 based on opposing evidence frequency).
- \(N\) = Number of references.
