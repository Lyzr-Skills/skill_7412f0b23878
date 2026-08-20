# Scoring Model

## ICP Fit Score
Calculates segment scoring across 10 core dimensions:
\[ \text{ICP Fit Score} = \sum (Dimension\_Score \times Configured\_Weight) \]

Core Dimensions:
1. Problem Severity (1-10)
2. Problem Frequency (1-10)
3. Product Fit (1-10)
4. Willingness to Pay (1-10)
5. Urgency (1-10)
6. Accessibility (1-10)
7. Market Size (1-10)
8. Competition (1-10)
9. Retention Potential (1-10)
10. Strategic Fit (1-10)

## Persona Priority Score
Calculates persona alignment in the B2B context:
\[ \text{Persona Priority Score} = \frac{\text{Pain Intensity} + \text{Decision Influence} + \text{Purchase Influence} + \text{Accessibility} + \text{Message Resonance}}{5} \]
Each element rated 1-10.
