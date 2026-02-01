# IBM watsonx Technical Implementation - GLPA System

## watsonx Orchestrate Configuration

### Workflow Architecture
- **Orchestrate App Name:** GLPA-Risk-Detection
- **Trigger:** Scheduled (Every 6 hours) + Manual
- **Skills Used:**
  - RSS Feed Reader (ReliefWeb API)
  - Text Analytics (Granite-13b-instruct-v2)
  - JSON Parser
  - Email Notification

### Agent Workflow Steps
1. **Data Ingestion Skill:** Connects to UN OCHA ReliefWeb API
2. **Signal Detection Skill:** Granite model analyzes text for risk indicators
3. **Ethics Validation Skill:** Second Granite instance removes bias
4. **Alert Generation Skill:** Formats output for human review

## watsonx.ai Foundation Model Usage

### Primary Model: granite-13b-instruct-v2
- **Temperature:** 0.3 (Low creativity for factual analysis)
- **Max Tokens:** 512
- **Top P:** 0.85

### API Integrations
- **ReliefWeb API:** https://api.reliefweb.int/v1/reports
- **ACLED Data:** CSV import via Orchestrate file connector
- **Output:** Slack webhook for NGO notifications
