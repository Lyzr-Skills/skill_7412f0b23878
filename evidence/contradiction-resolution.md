# Contradiction Resolution

Handles opposing evidence logs.

## Process
1. If conflicting records are found, group them by source type.
2. If first-party records conflict, trigger a split-segment logic check (to evaluate if the target ICP needs to be divided into separate distinct sub-segments).
3. If split-segment is not possible, assign status `"contradictory"` and apply a contradiction penalty to decay downstream confidence.
