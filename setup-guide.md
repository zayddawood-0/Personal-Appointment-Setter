# Setup Guide

This document explains how to configure and run the AI Appointment Setter Voice Agent using ElevenLabs, Cal.com, Google Calendar, and Salesforce CRM.

The project is built using a no-code workflow approach with AI-powered voice automation.

---

# Prerequisites

Before starting, make sure you have accounts for the following services:

| Service | Required |
|---------|----------|
| ElevenLabs | Yes |
| OpenAI | Yes |
| Cal.com | Yes |
| Google Account | Yes |
| Salesforce Developer Account | Yes |

---

# Project Overview

The setup process includes:

1. Creating the AI voice agent
2. Configuring conversational workflows
3. Connecting scheduling APIs
4. Connecting Google Calendar
5. Integrating Salesforce CRM
6. Testing the AI assistant

---

# Step 1 — Create ElevenLabs Account

## Website

https://elevenlabs.io/

---

## Instructions

1. Visit ElevenLabs
2. Create an account
3. Verify your email
4. Open the ElevenLabs dashboard

---

# Step 2 — Create AI Agent

## Instructions

1. Open:
```txt
ElevenLabs → Conversational AI → Agents
```

2. Click:
```txt
Create Agent
```

3. Configure:
- Agent name
- Voice model
- Personality
- Prompt instructions
- Workflow logic

---

## Recommended Agent Configuration

| Setting | Value |
|---------|-------|
| Agent Type | Appointment Setter |
| Voice Style | Professional |
| Tone | Friendly & Conversational |
| Language | English |
| Response Style | Human-like |

---

# Step 3 — Configure System Prompt

Add a detailed system prompt describing:
- AI behavior
- Conversation goals
- Booking logic
- Qualification logic
- Professional communication style

---

## Example Prompt Responsibilities

The assistant should:
- Greet users warmly
- Understand user requirements
- Qualify leads
- Check appointment availability
- Book meetings
- Handle follow-ups professionally

---

# Step 4 — Build Workflow

Inside ElevenLabs workflow builder:

Create nodes for:
- Greeting
- Qualification
- Availability checking
- Booking meetings
- Follow-up handling
- Wrap-up conversation

---

## Recommended Workflow Structure

```txt
Start
  ↓
Greeting
  ↓
Qualify Interest
  ↓
Check Availability
  ↓
Book Meeting
  ↓
Wrap Up
  ↓
End
```

---

# Step 5 — Connect Cal.com

## Purpose

Cal.com is used for:
- Checking available time slots
- Scheduling meetings
- Managing appointments

---

## Create Cal.com Account

Website:
https://cal.com/

---

## Generate API Key

### Instructions

1. Open:
```txt
Settings → Developer → API Keys
```

2. Click:
```txt
Create API Key
```

3. Copy the generated API key

---

## Add API Key in ElevenLabs

Inside the tool integration section:
- Select Cal.com
- Paste API key
- Save integration

---

# Step 6 — Connect Google Calendar

## Purpose

Google Calendar synchronizes meeting schedules automatically.

---

## Instructions

1. Open Cal.com
2. Navigate to:
```txt
Settings → Calendars
```

3. Connect Google Account
4. Allow permissions
5. Enable calendar sync

---

## Features Enabled

- Automatic event creation
- Real-time availability
- Meeting synchronization
- Conflict prevention

---

# Step 7 — Create Salesforce Developer Account

## Website

https://developer.salesforce.com/

---

## Instructions

1. Create free developer account
2. Verify email
3. Log into Salesforce dashboard

---

# Step 8 — Configure Salesforce Connected App

## Open Setup

Inside Salesforce:
```txt
Setup → App Manager
```

---

## Create External Client App

Click:
```txt
New External Client App
```

---

## Configure OAuth

### Callback URL

```txt
http://localhost:3000/callback
```

---

## OAuth Scopes

Add:
```txt
Full access (full)
Manage user data via APIs (api)
```

---

# Step 9 — Obtain Salesforce Credentials

After app creation:

Go to:
```txt
Settings → OAuth Settings
```

Copy:
- Consumer Key
- Consumer Secret

---

## Find Instance Hostname

Your instance hostname is:

```txt
yourcompany.my.salesforce.com
```

Example:
```txt
orgfarm-xxxx-dev-ed.develop.my.salesforce.com
```

---

# Step 10 — Connect Salesforce in ElevenLabs

Inside ElevenLabs tools section:

Paste:
- Instance Hostname
- Consumer Key
- Consumer Secret

Enable:
- salesforce_create_lead
- salesforce_get_contact
- salesforce_search

---

# Step 11 — Configure CRM Workflow

The AI assistant should:
- Create leads automatically
- Store customer details
- Save booking information
- Handle follow-up data

---

# Step 12 — Test Voice Agent

Test scenarios:
- Greeting conversation
- Lead qualification
- Appointment booking
- Calendar synchronization
- CRM updates
- Follow-up flow

---

# Step 13 — Publish AI Agent

After testing:

Click:
```txt
Publish
```

Your AI voice assistant is now live.

---

# Recommended Project Structure

```txt
AI-Appointment-Setter-Agent/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── workflow-explanation.md
├── integrations.md
├── setup-guide.md
├── architecture.md
│
├── screenshots/
│
└── demo/
```

---

# Optional Enhancements

You can further improve the project by adding:

- WhatsApp Integration
- Email Automation
- SMS Notifications
- Multi-language Support
- Analytics Dashboard
- RAG Knowledge Base
- Voice Cloning
- Admin Panel

---

# Troubleshooting

---

## Cal.com Not Connecting

### Solution
- Regenerate API key
- Verify permissions
- Reconnect integration

---

## Salesforce Authentication Failed

### Solution
- Verify Consumer Key
- Verify Consumer Secret
- Confirm OAuth scopes
- Check Instance Hostname

---

## Google Calendar Sync Issues

### Solution
- Reconnect Google account
- Enable calendar permissions
- Verify timezone settings

---

## AI Agent Not Responding Correctly

### Solution
- Improve prompt instructions
- Refine workflow logic
- Add better qualification prompts

---

# Security Best Practices

Never upload:
- API keys
- OAuth credentials
- Consumer secrets
- Access tokens

Use:
```txt
.env files
```
or secure credential managers.

---

# Deployment Recommendations

Recommended platforms:
- ElevenLabs
- Vercel
- Netlify
- Railway
- Render

---

# Conclusion

This setup creates a production-style AI appointment setter capable of:
- Handling natural conversations
- Automating scheduling
- Managing CRM workflows
- Synchronizing calendars
- Improving customer interaction

The project demonstrates modern AI automation using no-code tools and API integrations.
