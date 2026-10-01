# 🚀 AI-Powered Lead Generation Agent (n8n Workflow)

[![n8n.io](https://img.shields.io/badge/n8n-Workflow-FF6D5A?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Apify](https://img.shields.io/badge/Apify-Scraper-00C2FF?style=for-the-badge&logo=apify&logoColor=white)](https://apify.com)
[![Google Sheets](https://img.shields.io/badge/Google%20Sheets-Database-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)](https://workspace.google.com/products/sheets/)

An enterprise-grade, automated lead generation pipeline built on **n8n**. This workflow seamlessly extracts business data, filters junk records, performs AI-driven lead scoring, logs structured insights into Google Sheets, and sends instant HTML email alerts via Gmail.

---

## ✨ Key Features

* **⚡ Automated Data Extraction:** Triggered via Webhook to scrape real-time business data using Apify Actors.
* **🧹 Smart Data Filtering:** Automatically removes permanently/temporarily closed businesses to keep your pipeline clean.
* **🧠 AI Lead Scoring & Analysis:** Powered by OpenAI (LangChain Agent) to evaluate business potential, identify pain points, and suggest custom outreach angles.
* **📊 Automated Sheet Logging:** Saves clean, structured lead profiles into Google Sheets for easy CRM integration.
* **📧 Rich HTML Email Alerts:** Delivers beautifully formatted lead reports directly to your inbox using Gmail.

---

## 🛠️ Tech Stack & Integration

* **Orchestration:** n8n
* **Web Scraping:** Apify
* **AI & NLP:** OpenAI (GPT-4), LangChain
* **Storage & Outreach:** Google Sheets, Gmail API

---

## 🚀 Quick Start & Setup

### Prerequisites
1. An active **n8n** instance (Self-hosted or Cloud).
2. API Keys for **Apify** and **OpenAI**.
3. OAuth authentication setup for **Google Sheets** and **Gmail**.

### Installation
1. Clone or download this repository.
2. Open your n8n dashboard.
3. Click on **Workflows** > **Import from File**.
4. Select the `workflow.json` file from this project.
5. Connect your credentials for Apify, OpenAI, Google Sheets, and Gmail in the respective nodes.
6. Activate the workflow!

---

## 📥 Webhook Request Example

Send a `POST` request to your n8n Webhook URL with the following JSON payload:

```json
{
  "query": "Real Estate Agents",
  "location": "Miami, FL",
  "numberOfResults": 10,
  "Email": "your-email@example.com"
}
