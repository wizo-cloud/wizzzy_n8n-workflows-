🤖 AI Lead Qualification System — n8n + Gemini + Google Sheets + Slack + Gmail

Stop letting good leads go cold while your team manually sorts through tyre-kickers.


The Problem
You run an agency — real estate, marketing, SaaS, doesn't matter. Your website and ads are pulling in enquiries every day. But 70–80% of them aren't serious buyers. Tyre-kickers, people browsing, the occasional bot.
So what actually happens?
Someone on your team manually reviews every lead, copies data into a spreadsheet, tries to figure out who's worth calling, then fires off the same template reply — if they remember to reply at all.
A genuinely good lead sits untouched for hours. Sometimes longer.
Meanwhile, the person who was ready to buy has already moved on.

The Solution
I built an AI lead qualification system to stop that from happening.
The second a lead hits your form:

✅ It's captured and cleaned up automatically
✅ A Gemini AI agent scores it — High Intent, Nurture, or Cold — with actual reasoning behind the score
✅ The right follow-up email goes out immediately (no more forgotten replies)
✅ Everything lands in Google Sheets for your records
✅ When a high-priority lead comes in, Slack pings you straight away

No spreadsheet sorting. No chasing people who were never going to buy. No guessing.

How It Works
Enquiry Form Submission
        ↓
   n8n Webhook (captures lead instantly)
        ↓
   Set Node (cleans and structures data)
        ↓
   Gemini AI Agent (scores lead 1–10 with reasoning)
        ↓
   Structured Output Parser
        ↓
   ┌────────────────────────────────────┐
   │         3-Tier Switch Node         │
   │  High Intent (>7) | Nurture (4–7) | Cold (<4)  │
   └────────────────────────────────────┘
        ↓               ↓              ↓
  Slack Alert     Gmail Follow-up   Gmail Follow-up
  + Gmail         (nurture email)   (cold email)
        ↓
  Google Sheets (all leads logged with score + reasoning)

Tech Stack
ToolRolen8nWorkflow automation engineGoogle GeminiAI lead scoring agentGoogle SheetsLead database & CRM loggingGmailAutomated follow-up emailsSlackReal-time high-intent alerts

What You Get

Instant response — leads never sit unattended
AI reasoning — not just a score, but why the lead was scored that way
Three-tier routing — different follow-ups for different lead types
Full visibility — every lead logged with timestamp, score, and reasoning
Slack alerts — your team knows the moment a hot lead lands


How to Import Into n8n

Download the .json file from this repo
Open n8n → click "+" to create a new workflow
Click the menu (⋮) → "Import from file"
Select the downloaded .json file
Add your credentials to the relevant nodes:

Google Gemini API key
Gmail OAuth
Google Sheets OAuth
Slack Bot Token




Built By
Okafor Wisdom (Wizo) — AI Workflow Automation Developer
Specialising in n8n-based automation systems for SMBs.
📧 wisdomokafor47@gmail.com
🔗 LinkedIn

If your team is burning time on bad leads instead of working good ones, reach out. I'll show you exactly how it runs — and I'm happy to walk you through the template.


