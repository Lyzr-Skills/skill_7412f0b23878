# ICP & Persona Analysis Skill

A structured customer-intelligence engine that converts raw customer/market evidence into verified ICP and Persona outputs with confidence scoring.

## Folder Directory Sitemap

- [`skill.md`](file:///C:/Users/athar/OneDrive/Documents/projects/skills/ICP%20&%20Persona%20Analysis%20Skill/skill.md) - Main specification file.
- [`architecture.md`](file:///C:/Users/athar/OneDrive/Documents/projects/skills/ICP%20&%20Persona%20Analysis%20Skill/architecture.md) - Pipeline architecture layout.
- [`workflow.md`](file:///C:/Users/athar/OneDrive/Documents/projects/skills/ICP%20&%20Persona%20Analysis%20Skill/workflow.md) - Pipeline phase detailed workflow.
- `core/` - Intelligence engine core contracts, quality gates, and traceability rules.
- `evidence/` - Source weighting, classification taxonomy, and confidence math.
- `modules/` - Executable pipeline stages.
- `schemas/` - JSON schemas for inputs, intermediates, and final outputs.
- `prompts/` - LLM System instructions for each pipeline stage.
- `tests/` - Adversarial validation tests.
- `docs/` - System configuration and usage guides.

## Execution
This skill runs as a multi-stage pipeline. Execute stages sequentially or as a single composable pipeline via the Growth Strategy or Market Intelligence Agents.
