# AI Operator Stack - Notion Template Structure

## 📋 Operator Dashboard Template

Copy this structure into Notion to build your Operator Dashboard.

---

## Page 1: Dashboard (Home)

### Database: Quick Stats (Inline)
| Property | Type |
|----------|------|
| Revenue (MTD) | Number |
| Active Clients | Number |
| Tasks Open | Number |
| Next Action | Text |

### Sections:
- **Today's Focus** → Linked view: Tasks (Filter: Due Date = Today)
- **Upcoming Deadlines** → Linked view: Tasks (Filter: Due Date within 7 days)
- **Recent Client Activity** → Linked view: Clients (Sort: Last Contact descending)
- **Revenue This Month** → Formula or manual entry

---

## Page 2: Tasks & Projects

### Database: Tasks
| Property | Type | Options |
|----------|------|---------|
| Name | Title | |
| Status | Select | To Do, In Progress, Done, Waiting |
| Priority | Select | High, Medium, Low |
| Due Date | Date | |
| Project | Relation | → Projects |
| Client | Relation | → Clients |
| Time Estimate | Number | (minutes) |
| AI Assisted | Checkbox | |

### Database: Projects
| Property | Type |
|----------|------|
| Name | Title |
| Client | Relation → Clients |
| Status | Select (Active, Completed, On Hold) |
| Start Date | Date |
| Due Date | Date |
| Budget | Number |
| Tasks | Relation → Tasks |

---

## Page 3: Clients CRM

### Database: Clients
| Property | Type |
|----------|------|
| Name | Title |
| Company | Text |
| Email | Email |
| Phone | Phone |
| Status | Select (Lead, Active, Past) |
| Source | Select (Referral, Cold Outreach, Product Hunt, etc.) |
| Last Contact | Date |
| Projects | Relation → Projects |
| Invoices | Relation → Invoices |
| Notes | Text (long) |
| Tags | Multi-select |

### Views:
- **All Clients** → Table view
- **Leads** → Filter: Status = Lead
- **Active** → Filter: Status = Active
- **Needs Follow-up** → Filter: Last Contact > 30 days ago

---

## Page 4: Invoices & Finance

### Database: Invoices
| Property | Type |
|----------|------|
| Invoice # | Title (auto-increment) |
| Client | Relation → Clients |
| Amount | Number |
| Status | Select (Draft, Sent, Paid, Overdue) |
| Issue Date | Date |
| Due Date | Date |
| Paid Date | Date |
| Items | Text (or sub-items) |

### Finance Dashboard:
- Total Revenue (MTD) → Rollup: Sum of Invoices where Status = Paid
- Outstanding → Rollup: Sum where Status = Sent or Overdue

---

## Page 5: AI Prompts Library

### Structure:
Create a database "AI Prompts" or use simple pages organized by category:

#### 📝 Writing Prompts
- Cold Email Generator
- Follow-up Message
- Proposal Outline
- Case Study Writer

#### 📞 Client Communication
- Meeting Summary
- Scope Definition
- Contract Redline Request
- Feedback Request

#### 📊 Content Creation
- Blog Post Outline
- Social Media Thread
- Newsletter Draft
- Video Script Hook

#### 🔍 Analysis
- Competitor Research
- Pricing Strategy
- Business Metrics Review
- Contract Analysis

### Each Prompt Page Template:
```
## Prompt
[Copy-paste the actual prompt with {{brackets}} for variables]

## How to Use
- Best for: [use case]
- Replace: [variables to fill in]
- Expected output: [what you'll get]

## Example Output
[optional: show what it produces]
```

---

## Page 6: 30-Day Implementation Tracker

### Database: Implementation Tasks
| Property | Type |
|----------|------|
| Day | Number (1-30) |
| Task | Title |
| Category | Select (Setup, Automation, Content, etc.) |
| Status | Select (Pending, Done) |
| Notes | Text |

### Day-by-Day Guide:

#### Week 1: Foundation
1. Create Notion account + duplicate template
2. Set up Clients database with 5 current clients
3. Create your first project
4. Add 10 tasks for the week

#### Week 2: Automation Basics
5. Set up email capture form
6. Connect form to Notion (n8n workflow)
7. Create 3 AI prompt shortcuts
8. Test first automated workflow

#### Week 3: Content Engine
9. Set up content repurposing workflow
10. Create email sequence for leads
11. Build client onboarding template
12. Document standard responses

#### Week 4: Optimization
13. Review metrics and automate more
14. Set up invoice tracking
15. Create client portal/portal page
16. Plan next month's improvements

#### Days 17-30: Continue building out workflows based on what you use most.

---

## 🔗 Integrations

### n8n Connections:
- **Form** (Typeform/Lemon Squeezy) → n8n → Notion (New Client)
- **Invoice Paid** (Lemon Squeezy) → n8n → Notion (Update Status)
- **New Lead** (Twitter/Email) → n8n → Notion (Add to pipeline)

### AI Tools Integration:
- ChatGPT/Claude: Use prompts from Page 5
- Keyboard Maestro (Mac): Create shortcuts for common prompts
- Text Expander: Save prompt templates

---

## ✅ Quick Start Checklist

- [ ] Duplicate this template
- [ ] Add 5 current/past clients
- [ ] Add 3 active projects
- [ ] Create this week's task list
- [ ] Set up 3 AI prompts you use most
- [ ] Connect one automation (form → Notion)
- [ ] Test end-to-end flow

---

*Template created for AI Operator Stack - 2026*
