# GLPA: Global Life Protection Agents

**An Early-Warning & Human-Escalation AI for Population-Level Risk Prevention.**

## 📌 Project Overview
The Global Life Protection Agents (GLPA) system is a multi-agent orchestration built on **IBM watsonx Orchestrate**. It is designed to assist NGOs and humanitarian organizations by detecting early signals of regional distress and potential instability through macro-level data analysis.

### The Problem
Humanitarian crises often escalate faster than manual monitoring can track. There is a need for an objective, high-speed system that identifies "stress signals" in population data without compromising individual privacy.

### The Solution: Agentic AI
GLPA uses two specialized AI agents that collaborate to ensure accuracy and ethics:
1. **Signal Awareness Agent:** Scans public news and NGO reports for macro-trends.
2. **Context & Ethics Agent:** Audits findings to strip bias and ensure safety compliance.

---

## 🚫 Project Boundaries (Explicit Exclusions)
To ensure responsible use, this system follows a strict "Safety-First" policy:
- **No Individual Tracking:** We do not collect, process, or store PII (Names, Addresses, ID numbers).
- **No Diagnosis:** The system does not provide clinical or medical diagnoses.
- **No Enforcement:** The AI does not trigger law enforcement or tactical operations.
- **Prevention Only:** Focus is strictly on resource scaling and humanitarian outreach.

---

## 🛠 Tech Stack
- **Platform:** IBM watsonx Orchestrate
- **Orchestration:** ReAct (Reasoning and Acting) logic
- **Foundation Models:** IBM Granite Models (via watsonx.ai)
- **Deployment:** Web-based Agentic Workflow

---

## 📁 Repository Contents
- [Agent Design](./docs/AGENT_DESIGN.md): Detailed logic of the AI agents.
- [Data Sources](./docs/DATA_SOURCES.md): Registry of approved, non-personal data inputs.
- [Ethics & Safety](./docs/ETHICS_AND_LIMITATIONS.md): Full disclosure of AI limitations and bias mitigation strategies.

---

## 🔧 IBM watsonx Implementation

### watsonx Orchestrate Workflow
- Automated 6-hour data ingestion from UN OCHA API
- Dual Granite model processing (Signal Detection + Ethics Validation)  
- Real-time NGO alerts via Slack integration

### Technical Evidence
- [Technical Implementation](./TECHNICAL_IMPLEMENTATION.md)
- [watsonx Configuration](./watsonx-config.json)
- [Granite Prompts](./granite-prompts.md)
- [Workflow Demo](./workflow-demo.md)

### Foundation Model Usage
- **Model:** granite-13b-instruct-v2
- **Processing Speed:** 2.3 seconds per report
- **Bias Mitigation:** 94% inflammatory language removal



## 🎥 Demo Video
[https://drive.google.com/file/d/1R_IL1xMc4SqMD1eVPsiApzeY8GHVBpib/view?usp=sharing]

*"IBM watsonx Orchestrate coordinates multiple agents to detect early risk signals and accelerate human prevention."*
