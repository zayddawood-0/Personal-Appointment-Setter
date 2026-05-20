# AI Appointment Setter Voice Agent

An advanced no-code AI voice assistant built using ElevenLabs, Cal.com, Google Calendar, and Salesforce CRM to automate appointment scheduling and customer interactions in real time.

---

# Overview

This project is a conversational AI voice agent capable of handling natural voice conversations, scheduling appointments, checking availability, syncing meetings with Google Calendar, and managing customer data through Salesforce CRM.

The assistant is designed to simulate a professional AI receptionist or appointment setter for businesses, clinics, agencies, and customer support systems.

The complete workflow was created using modern no-code AI automation tools without building a traditional backend.

---

# Features

- Real-time AI voice conversations
- Human-like voice interaction
- Automated appointment scheduling
- Google Calendar synchronization
- Salesforce CRM integration
- AI-powered customer interaction
- Natural conversational responses
- No-code workflow automation
- Professional appointment management
- Multi-tool API integration
- AI receptionist workflow
- Smart scheduling assistant

---

# Tech Stack

| Technology | Purpose |
|------------|----------|
| ElevenLabs | Voice AI Agent |
| OpenAI | Conversational Intelligence |
| Cal.com | Appointment Scheduling |
| Google Calendar | Calendar Management |
| Salesforce CRM | Customer Relationship Management |
| Zapier / Webhooks | Automation Workflows |

---

# Workflow Architecture

```txt
User Voice Input
        ↓
ElevenLabs AI Voice Agent
        ↓
Conversational Processing
        ↓
Lead Qualification
        ↓
 ┌───────────────────────────────┐
 │ Qualified Prospect            │
 │               OR              │
 │ Not Ready Yet                 │
 └───────────────────────────────┘
        ↓                    ↓
Check Availability      Nurture Workflow
        ↓                    ↓
Book Meeting         Collect Follow-up Info
        ↓                    ↓
Wrap Up                  End
        ↓
End
```

---

# Workflow Explanation

## 1. Greeting Stage

The AI assistant starts the conversation with a warm and professional greeting.

### Purpose
- Welcome the prospect
- Build conversational comfort
- Introduce the assistant naturally

### Example
```txt
Hello! Thank you for reaching out.
I'd be happy to help you schedule an appointment today.
```

---

## 2. Interest Qualification

The assistant identifies:
- User intent
- Use case
- Timeline
- Interest level

### AI Actions
- Understand customer requirements
- Qualify the lead
- Determine readiness for booking

---

## 3. Decision Branching

The workflow splits into two paths:

### Qualified Prospect
If the prospect is ready:
```txt
→ Check Availability
```

### Not Ready Yet
If the prospect is interested but hesitant:
```txt
→ Nurture Workflow
```

---

## 4. Check Availability

The assistant checks available slots using Cal.com integration.

### Integrations Used
- Cal.com API
- Google Calendar Sync

### AI Actions
- Fetch available time slots
- Offer scheduling options
- Suggest meeting times

---

## 5. Book Meeting

After the user selects a slot, the assistant:
- Confirms appointment details
- Creates booking
- Stores meeting information

### Systems Involved
- Cal.com
- Google Calendar
- Salesforce CRM

---

## 6. Wrap Up

The AI assistant concludes the conversation professionally.

### AI Actions
- Confirm booking
- Thank the user
- End conversation naturally

---

## 7. Nurture Workflow

For prospects not ready to book immediately.

### AI Actions
- Maintain engagement
- Offer future follow-up
- Request contact information
- Collect email preferences

---

# Integrations Used

## ElevenLabs
Used for:
- AI voice generation
- Real-time conversations
- Conversational AI

Website:
https://elevenlabs.io/

---

## Cal.com
Used for:
- Appointment scheduling
- Availability checking
- Meeting automation

Website:
https://cal.com/

---

## Google Calendar
Used for:
- Calendar synchronization
- Event management
- Appointment tracking

Website:
https://calendar.google.com/

---

## Salesforce CRM
Used for:
- Customer management
- Lead storage
- CRM automation

Website:
https://www.salesforce.com/

---

# Project Screenshots

## ElevenLabs Dashboard
![ElevenLabs Dashboard](screenshots/elevenlabs-dashboard.png)

---

## Workflow Structure
![Workflow](screenshots/workflow.png)

---

## AI Agent Tools
![Tools Page](screenshots/tools-page.png)

---

## Salesforce Integration
![Salesforce Integration](screenshots/salesforce-integration.png)

---

## Cal.com Integration
![Cal.com Integration](screenshots/calcom-integration.png)

---

# Demo Video

Instagram Reel Demo:

https://www.instagram.com/reel/DYhp6pCIWUi/

---

# Repository Structure

```txt
AI-Appointment-Setter-Agent/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── agent-prompt.md
├── workflow-explanation.md
├── integrations.md
├── setup-guide.md
├── architecture.md
│
├── screenshots/
│   ├── elevenlabs-dashboard.png
│   ├── workflow.png
│   ├── tools-page.png
│   ├── salesforce-integration.png
│   └── calcom-integration.png
│
└── demo/
    └── demo-link.md
```

---

# Setup Guide

## Step 1 — Create ElevenLabs Account

Create an account:
https://elevenlabs.io/

---

## Step 2 — Configure AI Agent

Configure:
- System prompt
- Voice model
- Conversational behavior
- Workflow logic

---

## Step 3 — Connect Cal.com

Generate API keys and connect:
- Scheduling tools
- Appointment APIs
- Availability checking

---

## Step 4 — Connect Google Calendar

Sync Cal.com with Google Calendar to automate event creation.

---

## Step 5 — Configure Salesforce CRM

Create Salesforce Developer Account and configure:
- Consumer Key
- Consumer Secret
- OAuth Settings
- Instance Hostname

---

## Step 6 — Add Automation Tools

Configure:
- CRM actions
- Scheduling actions
- Workflow automations

---

# API Integrations

## Cal.com API
Used for:
- Fetching available slots
- Creating appointments
- Scheduling meetings

---

## Salesforce API
Used for:
- Creating leads
- Managing customer information
- CRM operations

---

## Google Calendar Integration
Used for:
- Event synchronization
- Calendar management
- Meeting automation

---

# Business Use Cases

This AI assistant can be used for:

- AI Receptionists
- Appointment Scheduling
- Clinic Booking Systems
- Sales Automation
- Customer Support
- CRM Automation
- AI Front Desk Systems
- Consultation Booking
- Service-Based Businesses

---

# Skills Demonstrated

This project demonstrates practical implementation of:

- Conversational AI
- Voice AI Systems
- Prompt Engineering
- Workflow Automation
- API Integration
- CRM Automation
- No-Code AI Development
- AI Scheduling Systems
- Business Automation

---

# Future Improvements

Planned future upgrades:

- WhatsApp Integration
- Email Automation
- SMS Notifications
- Multi-language Support
- Voice Cloning
- Analytics Dashboard
- AI Memory System
- Admin Dashboard
- Lead Scoring System
- RAG-Based Knowledge Base

---

# Security Note

Sensitive credentials such as:
- API keys
- OAuth tokens
- Consumer secrets

are excluded from this repository for security purposes.

---

# Author

## Zayd Dawood

- AI & Automation Enthusiast
- Cybersecurity Enthusiast
- Voice AI Developer

---

# License

This project is licensed under the MIT License.

---
