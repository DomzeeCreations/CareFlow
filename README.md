# CareFlow

### AI-Powered Church Attendance, Forms & Follow-Up Intelligence System

> **CareFlow tells your church who needs attention, why they need it, who should reach out, what to do next, and when to follow up again.**

CareFlow combines attendance capture, custom forms & events, and care intelligence around a central **People Database** to help churches move from simply recording information to actively understanding, engaging, and caring for people.

Core loop: **Capture → Understand → Prioritize → Act → Follow Up → Learn**

---

## The Problem

Churches use separate tools for attendance, event registration, first-timer forms, membership info, follow-up, surveys, department registrations, conferences, and volunteer registration.

This creates fragmented information — one person in a form platform, attendance in another system, follow-up notes somewhere else.

CareFlow brings attendance, forms, events, people, and follow-up together in one connected system. The goal is not to collect more data. The goal is to help the church **understand and care for its people better.**

## Product Vision

Help churches move from simply recording information to **actively understanding, engaging, and caring for people through connected data and intelligent follow-up.**

## How It Works

### Layer 1: People Database

Central record for everyone connected to the church. Each profile connects to:

- Attendance
- Forms & submissions
- Events
- Cells / Small Groups
- Departments / Units
- Ministries
- Care Cases
- Follow-up history

### Layer 2: Attendance & Forms

Capture attendance and other information directly from members, visitors, and participants via links and QR codes.

### Layer 3: AI Intelligence

Analyze attendance, engagement, form data, and follow-up history to identify meaningful patterns — drops, absence, first-timers not returning, re-engagement, requests for contact.

### Layer 4: Care & Follow-Up

Turn insights into assigned actions, conversations, notes, reminders, and care cases.

Full loop: **Capture → Connect → Detect → Prioritize → Explain → Assign → Recommend → Follow Up → Record → Schedule → Reassess → Learn**

---

## Features

### A. People & Attendance

- Central People Database with Care Profiles
- Phone lookup with **shared phone number support** (one number → multiple people, e.g. families)
- Phone is used for lookup, not as unique identity
- First-timer registration: Scan → I'm New → Basic info → Recorded → Person created → Follow-up started
- Configurable church structure: Branch/Campus, Cell/Small Group, Department/Unit, Ministry, Service, custom groups
- Service creation & scheduling (Sunday, Midweek, Youth, Workers' Meeting, Vigil, Conference, custom)
- Automatic attendance link + QR code per service session
- Fast check-in: Scan QR → Identify yourself → Confirm → Recorded
- Duplicate attendance protection, attendance history, branch/campus support
- Attendance intelligence: sudden drops, repeated absence, first-timers not returning, new members going inactive, return after absence, positive re-engagement

### B. Forms & Events

- No-code Form Builder: Create Form → Add Fields → Configure → Publish → Share
- Field types: short/long text, number, phone, email, date, dropdown, multiple choice, checkbox, yes/no, file upload
- **Profile Fields vs Form/Event Fields:**
  - Profile: DOB, occupation, address, emergency contact → becomes part of Care Profile
  - Event: T-shirt size, accommodation, meal preference, track, volunteer role → stays with submission
- Shareable form link + QR code, start/end dates, confirmation message, submission settings
- Standard fields (name, phone, email) map to People Database
- Duplicate prevention (phone + email + name) with manual review — phone alone never auto-decides identity
- Event management: name, date, location, registration form, attendance, participants
- Form-triggered follow-up: e.g. "I would like someone to contact me" → Care Case
- Forms dashboard: active/draft/closed, submission counts, recent submissions
- Each submission stores: person, form, timestamp, responses, related event

### C. Care Intelligence

- Signals: attendance, new-member status, engagement (cell/department/ministry/event), follow-up history, leader-recorded care info, configured form responses
- Priority levels with explanations:
  - **High:** requires prompt attention
  - **Medium:** should receive attention soon
  - **Monitor:** worth watching
  - **Positive Engagement:** positive change
  - Example: "John usually attends Sundays. He has missed the last 2 Sundays with no follow-up in 14 days."
- **Care Cases** (AI or manual): first-timer, repeated absence, new member, pastoral care, check-in, event follow-up, contact request, manual concern
- Case contains: person, type, priority, reason, owner, status, recommended action, history, notes, next date, escalation, resolution
- Relationship-based assignment: 1. Cell Leader → 2. Dept/Unit Leader → 3. Care Team → 4. Pastoral Team (on escalation)
- Guided follow-up with context, not just "Call John" — why, recommended action, conversation approach
- Primary action MVP: phone call with outcomes (reached, no answer, call back, okay, needs support, needs pastoral, wrong number, other) + notes
- Automatic next follow-up suggestion (e.g. "Call back in 3 days"), editable
- Escalation: Monitor → Attention → Follow-Up Required → Escalation
- AI explains: what was detected, what contributed, why prioritized, what to do
- **AI assists. Humans decide.** No autonomous sensitive judgments about faith, emotional state, or personal circumstances.

### Action-First Dashboard

Answers: **"What do I need to do today?"**

- Today's Action List (e.g. "5 people need follow-up today")
- High Priority, Follow-Up Due, New People, Positive Engagement
- Recent Attendance, Open Care Cases, Recent Form Submissions, Active Events

Analytics exist, but action is primary.

## Product Philosophy

- **People Before Data**
- **Action Before Analytics** — "Who needs attention today?"
- **One Connected System**
- **AI Assists, Humans Decide**
- **Explain Important Recommendations**
- **Close the Loop** — every interaction has a clear next step

## Roadmap

MVP is A + B + C above.

Post-MVP possibilities:

- WhatsApp / SMS / Email follow-up
- Advanced event management, conditional form logic
- Automated reminders, workflows
- Advanced analytics & reporting
- Attendance kiosks, household management
- Mobile apps, deeper integrations

## Project Status

Early scaffolding. `main` currently holds this README. Implementation follows `Careflow PRD.md` (44 sections, full spec for People, Attendance, Forms, Events, Intelligence, Care Cases, Dashboard).

## Getting Started

Stack and setup to be decided. Planned:

```bash
# TBD
git clone https://github.com/DomzeeCreations/CareFlow.git
cd CareFlow
# install / dev commands coming
```

See `Careflow PRD.md` (in parent folder, not yet in repo) for full requirements.

## Contributing

Issues and PRs welcome. Please keep PRs focused, explain the care problem being solved, and avoid adding event-specific questions to core profile models — keep Profile vs Form field separation.

## License

TBD
