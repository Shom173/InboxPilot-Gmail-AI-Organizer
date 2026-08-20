# 📬 InboxPilot — Gmail AI Organizer

InboxPilot is an AI-powered Gmail automation built with **n8n and Gemini** that intelligently classifies incoming emails and organizes them using Gmail labels.

It supports both **real-time organization of new emails** and **controlled batch processing of existing inbox messages**, with rate-limit-aware processing for AI requests.

## ✨ Features

- 🤖 AI-powered email classification using Gemini
- 📩 Automatically processes new incoming emails
- 📦 Organizes existing inbox messages in batches
- 🏷️ Categorizes emails into:
  - IMPORTANT
  - JOBS
  - PERSONAL
  - FINANCE
  - EDUCATION
  - EVENTS
- ⚡ Controlled processing to reduce API rate-limit issues
- 🔄 Gmail + n8n workflow automation

## 🛠️ Tech Stack

- **n8n** — Workflow automation
- **Google Gemini** — AI email classification
- **Gmail API** — Email retrieval and labeling

## ⚙️ Workflow

```text
New Email
   ↓
Gmail Trigger
   ↓
AI Classification
   ↓
Category Routing
   ↓
Apply Gmail Label

Existing mail:

Manual Trigger
   ↓
Fetch Emails
   ↓
Process in Batches
   ↓
AI Classification
   ↓
Apply Gmail Label
   ↓
Wait / Rate Limit Control
```

## 🔐 Setup

- Import the workflow JSON into n8n.
- Connect your Gmail account.
- Configure your Gemini credentials.
- Create/select the required Gmail labels.
- Activate the workflow.

API keys and credentials are not included in this repository.
