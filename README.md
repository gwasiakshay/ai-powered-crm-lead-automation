🚀 AI-Powered CRM Lead Automation (n8n + OpenAI)

An end-to-end AI-powered CRM automation system built using n8n, OpenAI, and Google Sheets to intelligently classify, route, and manage incoming leads.

This project simulates an Intercom-style AI support & sales router, capable of:

Understanding user intent

Prioritizing leads

Routing to Sales / Support / Manual Review

Logging all actions automatically

🧠 Features

✅ AI-powered lead classification
✅ Intent detection (Sales / Support / General)
✅ Priority & lead score generation
✅ Automated routing logic
✅ Google Sheets integration
✅ Manual review fallback
✅ Fully no-code / low-code (n8n)
✅ Production-ready workflow structure


🏗️ Architecture Overview

Webhook (Lead Intake)
        ↓
Normalize Lead Data
        ↓
OpenAI GPT Classification
        ↓
AI Response Parser
        ↓
Confidence Check
        ↓
Intent Routing
   ├── Sales → Sales Sheet
   ├── Support → Support Sheet
   ├── Low Priority → Low Priority Sheet
   └── Low Confidence → Manual Review


📁 Project Structure

n8n-ai-powered-crm-lead-automation/
│
├── workflows/
│   └── AI-Powered CRM Lead Automation.json
│
├── screenshots/
│   └── workflow-diagram.png
│   └── Leads.png
│   └── low-priority-lead.png
│   └── Support.png
│
└── README.md
└── Tests.md


🔗 Webhook Testing

Example: Sales Lead
curl -X POST http://localhost:5678/webhook-test/<your-id> \
-H "Content-Type: application/json" \
-d '{
  "name": "John Doe",
  "email": "john@acme.com",
  "company": "Acme Corp",
  "message": "We want to automate our CRM",
  "source": "Website"
}'

Example: Support Request
{
  "name": "Sarah Lee",
  "email": "sarah@company.com",
  "message": "Dashboard not loading",
  "source": "App"
}

Example: Low Priority
{
  "name": "Mark",
  "email": "mark@gmail.com",
  "message": "Just exploring your services",
  "source": "Website"
}


🧠 Skills Demonstrated

AI workflow design

LLM prompt engineering

Automation logic

API integration

Data normalization

Production-ready n8n pipelines

Real-world CRM logic

🚀 Next Improvements (Planned)

 Slack / Email notifications

 Confidence threshold tuning

 Retry & error handling

 Logging dashboard

 Vector memory (future RAG upgrade)

 Docker deployment

 
👨‍💻 Author

Akshay Gwasikoti
AI Automation Engineer
🔗 GitHub: github.com/gwasiakshay