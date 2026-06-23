# AI Component Inventory

Use only if the project uses AI/ML models, LLM APIs, computer vision models, AI-assisted alerts, AI-generated commands, or AI-enabled user interfaces.

| Component | Type | Provider/source | Version/model ID | Input data | Output/action | Sensitive data? | Safety role? | Notes |
|---|---|---|---|---|---|---|---|---|
| | model/API/package | | | | | Yes/No | Advisory/Control/None | |

## Required checks

- [ ] AI is not the sole authority for safety-critical physical actuation.
- [ ] Model/API failure defaults to a safe device state.
- [ ] Prompts, logs, training data, and inference data are reviewed for sensitive content.
- [ ] AI dependencies are included in dependency scanning and SBOM notes.
