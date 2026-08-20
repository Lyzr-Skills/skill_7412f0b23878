# Disconfirming Evidence

Enforces active searches for evidence that invalidates current segments.

## Strategy
- The system must explicitly search for negative user reviews, churn logs, or cancellation tickets matching candidate segment dimensions.
- If negative reports are found, log under disconfirming evidence keys and subtract from product-fit scoring.
