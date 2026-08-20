# Core Intelligence Pipeline

The pipeline is orchestrating analysis stages sequentially. Each stage consumes the output file from the prior stage, validates it against schemas, and writes the structured result for downstream stages.

## Stage Interfaces
- `Stage 1: Context Analysis` -> outputs `context.json`
- `Stage 2: Customer Evidence Collection` -> reads `context.json`, outputs `evidence.json`
- `Stage 3: Signal Extraction` -> reads `evidence.json`, outputs `customer-signal.json`
- `Stage 4: Segment Discovery` -> reads `customer-signal.json`, outputs `segment.json`
- `Stage 5: Segment Comparison & ICP Scoring` -> reads `segment.json`, outputs comparison matrices
- `Stage 6: ICP Selection & Drift` -> outputs `icp.json` and checks `icp-snapshot.json`
- `Stage 7: Persona & Buying Committee` -> reads `icp.json`, outputs `persona.json` and `buying-role.json`
- `Stage 8: Pain & Trigger Analysis` -> outputs trigger and pain metrics
- `Stage 9: Journey, Objection & Channel Analysis` -> outputs mapping objects
- `Stage 10: Messaging & Executive Report` -> outputs unified `analysis-report.json`
