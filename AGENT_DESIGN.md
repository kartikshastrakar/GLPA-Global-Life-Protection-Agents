# Agent Responsibility Document

This document maps the technical roles of the agents within the watsonx Orchestrate environment.

### Agent 1: Signal Awareness (The Scanner)
- **Role:** Pattern Detection.
- **Input:** Aggregated News/NGO Summaries.
- **Output:** Trend JSON (Region, Indicators, Confidence).
- **Constraint:** Redacts all individual names.

### Agent 2: Context & Ethics (The Auditor)
- **Role:** Bias Mitigation & Validation.
- **Input:** Output from Agent 1.
- **Output:** Validated Briefing.
- **Logic:** Compares data against the Ethics Framework to neutralize sensationalist language.

### Orchestration Rule
`If Severity >= Medium -> Trigger Human Escalation Alert`