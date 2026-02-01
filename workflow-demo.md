# GLPA Workflow Demonstration

## Live watsonx Orchestrate Flow

### Step 1: Data Ingestion
- **Source:** UN OCHA ReliefWeb API
- **Frequency:** Every 6 hours
- **Filter:** Conflict and disaster reports from last 24h

### Step 2: Signal Detection (Granite Model)
**Input:** Raw humanitarian report text
**Output:** Structured risk assessment JSON

Example:
```json
{
  "region": "Eastern Ukraine",
  "risk_level": "high",
  "indicators": ["displacement surge", "infrastructure damage", "supply disruption"],
  "confidence": 0.89
}
