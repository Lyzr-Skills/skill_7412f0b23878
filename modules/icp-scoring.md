# ICP Scoring Module

Calculates segment scores using configured weights in `config/scoring.yaml`.

## Process
1. Query weights for the 10 core dimensions.
2. Formulate segment scores out of 100.
3. Classify into Primary ICP (min threshold), Secondary ICP, and Disqualified/Avoid segments.
