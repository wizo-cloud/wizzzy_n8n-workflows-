# 🤖 Autonomous LinkedIn Prospecting & Lead Intelligence System

An end-to-end AI-powered lead generation and outreach automation built with **n8n**, **Google Gemini**, **Apify**, **Google Sheets**, **Slack**, and **Gmail** — designed to help businesses find, qualify, and engage ideal prospects on LinkedIn without manual effort.

---

## 😩 The Problem

Finding quality leads on LinkedIn is painfully manual. Sales teams and founders spend **hours every day**:

- Scrolling through LinkedIn searching for the right prospects
- Copy-pasting names, titles, and companies into spreadsheets
- Guessing which leads are actually worth pursuing
- Writing and sending outreach one by one — only to get ignored

The result? Wasted time, inconsistent outreach, and a pipeline that depends entirely on human effort to keep moving.

---

## ✅ The Solution

This system **eliminates manual prospecting entirely.** It runs on a schedule, finds your ideal clients on LinkedIn, scores them with AI, and sends personalized outreach — all without you lifting a finger.

You wake up to a Slack notification: *"3 high-value leads found and contacted."*

## 🔗 Try It Live

👉 [Launch the LinkedIn Prospecting Form](https://n8n.srv1290655.hstgr.cloud/form/ca7f4927-5817-411e-b630-9796aed1c9d2)

Enter a LinkedIn search URL and watch the system qualify and score leads automatically.

---

![Workflow Screenshot](<Screenshot From 2026-04-07 10-47-53.png>)

---

## 🚀 What This System Does

This workflow autonomously:

1. **Scrapes LinkedIn profiles** matching a target ICP (Ideal Customer Profile) using Apify
2. **Qualifies each lead** using Google Gemini AI — scoring them by relevance, seniority, and fit
3. **Enriches lead data** (name, title, company, email where available) and logs to Google Sheets
4. **Sends personalized outreach emails** via Gmail based on qualification tier
5. **Notifies the team on Slack** when a high-value lead is identified

---

## 🧰 Tech Stack

| Tool | Role |
|------|------|
| **n8n** | Workflow orchestration |
| **Apify** | LinkedIn profile scraping |
| **Google Gemini** | AI lead qualification & scoring |
| **Google Sheets** | Lead database & deduplication |
| **Gmail** | Personalized outreach emails |
| **Slack** | Real-time team notifications |

---


## ✨ Key Features

- **AI-Powered Scoring** — Gemini evaluates each lead against configurable ICP criteria and assigns a qualification tier
- **Auto Deduplication** — Prevents re-contacting the same lead across multiple runs
- **Tiered Outreach** — Different email templates for High, Nurture, and Cold leads
- **Real-time Alerts** — Slack notifications fire instantly when a hot lead is found
- **Full Audit Trail** — Every lead, score, and action is logged to Google Sheets

---


## ⚙️ Setup Instructions

### Prerequisites
- n8n (self-hosted or cloud)
- Apify account + API key
- Google Cloud account (Gemini API key)
- Gmail account (OAuth2 connected in n8n)
- Slack workspace + bot token
- Google Sheets (with edit access)

### Steps

1. **Import the workflow** — Open n8n → Menu (⋮) → Import from File → select `workflow.json`
2. **Configure credentials** in n8n:
   - Apify API Key
   - Google Gemini (via HTTP Header Auth)
   - Gmail (OAuth2)
   - Google Sheets (OAuth2)
   - Slack (Bot Token)
3. **Set your ICP** — Update the Gemini system prompt inside the AI Qualification node with your target industry, title, and company size
4. **Set your Google Sheet ID** — Paste your Sheet ID into the Google Sheets nodes
5. **Activate the workflow** — Switch to Production and enable the Schedule Trigger

---

## 📊 Results / Use Case

Built as a portfolio project demonstrating autonomous B2B prospecting. This system can:

- Process **100+ LinkedIn profiles per run**
- Reduce manual prospecting time by **~80%**
- Deliver qualified leads directly into your CRM or outreach tool

---

## 👤 Built By

**Okafor Wisdom (Wizo)**
AI Workflow Automation Developer · n8n Specialist

- 🌐 [LinkedIn](https://www.linkedin.com/in/okafor-wisdom-26a6962bb/)
- 📧 wisdomokafor47@gmail.com

---

## 📄 License

This project is for portfolio and demonstration purposes.
