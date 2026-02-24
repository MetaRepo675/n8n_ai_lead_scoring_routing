# AI-Powered Lead Scoring & Routing with n8n

This project is a professional workflow in n8n that automatically receives incoming leads from website forms, analyzes them using artificial intelligence (OpenAI), and routes them to appropriate paths based on the score obtained.

 ## Features
- Data fetch via Webhook (suitable for connecting to website forms)
- Data validation and normalization (preventing incomplete data)
- Metadata enrichment (company email detection, message length)
- Intelligent analytics with OpenAI (scoring, intent detection, summarization)
- Automated routing based on score:
- **High score (≥80):** Create deal in HubSpot + Notification in Slack
- **Medium score (40-79):** Save to Google Sheets + Create email draft in Gmail
- **Low score (<40):** Archive (log only)
- Error handling and safe fallback

## Prerequisites
- n8n installation (local or cloud) - [Guide](https://docs.n8n.io/hosting/installation/)
- OpenAI account with API key
- HubSpot account (optional) with API key
- Slack app and Webhook URL  (Optional)
- Google account with access to Sheets and Gmail
- Telegram bot token (if you want to use Telegram)

## Installation and setup

1. Clone this repository:
```bash
git clone https://github.com/yourusername/n8n-ai-lead-scoring.git
cd n8n-ai-lead-scoring
