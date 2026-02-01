# GLPA Deployment Guide

## watsonx Orchestrate Setup
1. Import `watsonx-config.json` into Orchestrate
2. Configure API credentials for ReliefWeb
3. Set up Slack webhook for notifications
4. Test workflow with sample data

## Required watsonx Services
- **watsonx Orchestrate:** Workflow automation
- **watsonx.ai:** Granite model access
- **Watson Studio:** Model fine-tuning (optional)

## Environment Variables
```bash
RELIEFWEB_API_KEY=your_api_key
SLACK_WEBHOOK_URL=your_webhook
WATSONX_API_KEY=your_watsonx_key
