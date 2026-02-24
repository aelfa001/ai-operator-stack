# AI Operator Stack - n8n Workflows Library

## 📦 Included Workflows (20+)

Each workflow includes step-by-step setup instructions and video walkthroughs.

---

## Core Workflows

### 1. Lead Capture → Notion
**What it does:** Auto-adds new leads from forms to your Notion CRM

**Trigger:** Webhook (Typeform, Google Forms, or custom form)

**Steps:**
1. Webhook receives form submission
2. Create Notion page in "Clients" database
3. Set status to "Lead"
4. Add tag based on source
5. Send Slack notification

**Setup Time:** 15 minutes

---

### 2. Invoice Status Tracker
**What it does:** Monitors payment status and updates Notion automatically

**Trigger:** Lemon Squeezy / Stripe webhook

**Steps:**
1. Listen for payment events
2. Find invoice in Notion
3. Update status (Sent → Paid/Overdue)
4. Calculate revenue metrics
5. Notify via Slack if overdue

**Setup Time:** 20 minutes

---

### 3. Content Repurposing Engine
**What it does:** Turns one piece of content into 10+ posts

**Trigger:** Manual (paste your content)

**Steps:**
1. Input: Blog post / video transcript / tweet thread
2. AI extracts key points
3. Generates:
   - LinkedIn post
   - Twitter thread
   - Instagram caption
   - Newsletter snippet
   - Email teaser
4. Saves to Notion "Content" database

**Setup Time:** 30 minutes

---

### 4. Client Onboarding Automation
**What it does:** Sends welcome sequence when new client added

**Trigger:** Notion "Client" status changes to "Active"

**Steps:**
1. Watch for new active client
2. Send welcome email (with attachments)
3. Create project in Notion
4. Add onboarding tasks to calendar
5. Send Slack to team

**Setup Time:** 25 minutes

---

### 5. Meeting Notes → Summary → Tasks
**What it does:** Auto-transcribes and creates action items

**Trigger:** New entry in Notion "Meeting Notes"

**Steps:**
1. Detect new meeting notes page
2. Send to AI for summary
3. Extract action items
4. Create tasks in Notion
5. Schedule follow-up

**Setup Time:** 20 minutes

---

## Communication Workflows

### 6. Email Lead Follow-up
**What it does:** Follows up with leads automatically

**Trigger:** Schedule (every day at 9am)

**Steps:**
1. Find leads with "No response in 3 days"
2. Personalize follow-up using AI
3. Send via Gmail
4. Log to Notion

---

### 7. Cold Email Outreach
**What it does:** Personalized outreach at scale

**Trigger:** Manual (upload CSV of prospects)

**Steps:**
1. Read prospect data
2. Generate personalized email using AI
3. Send via Gmail
4. Log to Notion
5. Add to follow-up sequence

---

### 8. Testimonial Request
**What it does:** Asks clients for reviews after project completion

**Trigger:** Project status = "Completed"

**Steps:**
1. Trigger after project completion
2. Personalize request email
3. Send to client
4. Track response in Notion

---

## Social Media Workflows

### 9. Twitter Engagement Auto-Responder
**What it does:** Replies to mentions with value

**Trigger:** New Twitter mention

**Steps:**
1. Detect new mention
2. Generate contextual reply with AI
3. Post reply
4. Log to Notion

---

### 10. LinkedIn Post Scheduler
**What it does:** Queues and posts content

**Trigger:** New entry in Notion "Content Queue"

**Steps:**
1. Read content from Notion
2. Format for LinkedIn
3. Schedule post via LinkedIn API
4. Update status in Notion

---

### 11. Instagram Story Reshare
**What it does:** Turns client DMs into stories

**Trigger:** New DM (via Instagram API)

**Steps:**
1. Detect new DM
2. AI generates caption
3. Create draft post
4. Notify to review

---

## Data & Analytics

### 12. Weekly Business Review
**What it does:** Compiles weekly metrics automatically

**Trigger:** Schedule (every Monday)

**Steps:**
1. Pull data from Notion
2. Calculate: revenue, tasks completed, new leads
3. Generate AI insights
4. Create weekly review page in Notion
5. Send summary email

---

### 13. Competitor Alert
**What it does:** Monitors competitor activity

**Trigger:** Schedule (daily)

**Steps:**
1. Search for competitor mentions
2. Summarize news
3. Add to Notion "Competitor Research"
4. Alert if significant

---

### 14. Lead Scoring
**What it does:** Ranks leads by likelihood to convert

**Trigger:** New lead added OR daily batch

**Steps:**
1. Pull lead data
2. Score based on: source, company size, activity
3. Update score in Notion
4. Flag hot leads for priority follow-up

---

## Operational

### 15. File Organization
**What it does:** Auto-organizes uploaded files

**Trigger:** New file in Google Drive / Dropbox

**Steps:**
1. Detect new file
2. Read filename/metadata
3. Move to correct folder
4. Add entry to Notion "Files"
5. Notify if attention needed

---

### 16. Calendar Sync
**What it does:** Bi-directional calendar sync with Notion

**Trigger:** Calendar event or Notion change

**Steps:**
1. Watch Notion for task dates
2. Create calendar events
3. Or: Watch calendar → create Notion tasks
4. Keep both in sync

---

### 17. Deadline Reminder
**What it does:** Proactive deadline notifications

**Trigger:** Schedule (daily at 8am)

**Steps:**
1. Find tasks due in next 3 days
2. Group by priority
3. Send summary email/Slack
4. Escalate overdue items

---

### 18. Client Portal Generator
**What it does:** Creates client-facing view

**Trigger:** New project created

**Steps:**
1. Generate unique page for client
2. Link to their project/notes
3. Share via magic link
4. Track access

---

## Advanced

### 19. AI Meeting Assistant
**What it does:** Joins meetings (Zoom/Google) and takes notes

**Trigger:** Calendar event starts

**Steps:**
1. Detect meeting start
2. Join as bot (with permission)
3. Record audio
4. Transcribe after
5. Generate summary + tasks in Notion

---

### 20. Proposal Generator
**What it does:** Creates proposals from templates

**Trigger:** Manual trigger with client info

**Steps:**
1. Input: Client name, project details
2. Generate proposal using AI
3. Create in Notion
4. Send via email
5. Track opens/clicks

---

### 21. Contract Redline Detector
**What it does:** Reviews contracts for red flags

**Trigger:** New file uploaded

**Steps:**
1. Upload PDF contract
2. AI extracts key clauses
3. Flag concerning terms
4. Summarize in Notion

---

### 22. Exit Interview Analyzer
**What it does:** Analyzes why clients churn

**Trigger:** Client status → "Churned"

**Steps:**
1. Pull client notes/history
2. Send exit survey if not done
3. Analyze feedback with AI
4. Create churn report
5. Suggest improvements

---

## 🚀 Quick Start: Your First 3 Workflows

Start with these to see immediate results:

1. **Lead Capture → Notion** (15 min)
2. **Content Repurposing** (30 min)  
3. **Weekly Business Review** (20 min)

---

## 🔧 Prerequisites

- **n8n** (self-hosted or cloud) - Free tier works
- **Make.com** alternative - Also included
- **Notion** - Free personal plan
- **Gmail** - For sending emails
- **Slack** (optional) - For notifications

---

## 📹 Setup Videos

Each workflow includes:
- 5-10 minute video walkthrough
- Written guide
- Troubleshooting tips
- Copy-paste code blocks

---

*Workflows library for AI Operator Stack - 2026*
