# Thari Tech CRM

A comprehensive, production-ready CRM demo built for Thari Tech — modelled after Zoho CRM and HubSpot. Built as a single-file HTML application with zero dependencies, designed to demo to enterprise clients.

**Live demo:** (https://unam-spec.github.io/thari-tech/)

---

## Features

**8 fully navigable modules:**

- **Dashboard** — KPI cards, recent deals table, live activity feed, rep performance bars, lead source breakdown, and today's task widget with a personalized welcome banner
- **Pipeline** — 6-stage Kanban board (Lead → Qualified → Meeting → Proposal → Negotiation → Closed Won) with deal cards showing value, owner, and color-coded age indicators
- **Contacts** — Card grid with deal count, total value, last contact date, lead status badges, and quick Email / Call / View actions
- **Companies** — Full table view with industry, contact count, open deals, deal value, and activity status
- **Deals** — List view with win probability bars, stage badges, and deal health indicators
- **Tasks** — Interactive checklist with priority levels, upcoming meetings panel, and a task summary widget. All checkboxes are fully clickable
- **Email Sequences** — Sequence cards with step-by-step flow visualization, open rate, reply rate, and conversion metrics
- **Reports & Analytics** — Monthly revenue bar chart, deals-by-stage funnel, rep leaderboard, lead source breakdown, and email performance stats

**UI features:**

- Notification bell with unread dropdown
- Quick Add button with 4 shortcuts (Contact, Deal, Task, Sequence)
- Full create/view modals for every entity
- Pill filters on Contacts and Deals views
- Responsive sidebar navigation with active state
- South African market data (ZAR pricing, local names and companies)

---

## Tech Stack

- Vanilla HTML, CSS, JavaScript — zero frameworks, zero dependencies
- Google Fonts (Plus Jakarta Sans)
- Deployed via GitHub Actions to GitHub Pages

---

## Getting Started

### Run locally

```bash
# Clone the repo
git clone https://github.com/Unam-spec/estateiq-crm.git
cd estateiq-crm

# Open in browser — no build step needed
open index.html
```

### Deploy to GitHub Pages

Push to `main` and GitHub Actions handles the rest. Make sure GitHub Pages is enabled:

1. Go to **Settings → Pages**
2. Set Source to **Deploy from a branch**
3. Select **main** branch, **/ (root)** folder
4. Save — your site will be live at `https://unam-spec.github.io/estateiq-crm/`

---

## Project Structure

```
estateiq-crm/
├── index.html          # Full CRM application (single file)
├── README.md           # This file
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions auto-deploy workflow
```

---

## Modules Overview

| Module          | Records  | Key Actions                            |
| --------------- | -------- | -------------------------------------- |
| Dashboard       | —        | View KPIs, activity, tasks             |
| Pipeline        | 24 deals | Kanban view, create deal               |
| Contacts        | 1,284    | Filter, view profile, email/call       |
| Companies       | 284      | Table view, add company                |
| Deals           | 42       | Filter by status, probability tracking |
| Tasks           | —        | Check off tasks, view meetings         |
| Email Sequences | 3        | View steps, open/reply rates           |
| Reports         | —        | Revenue, win rate, rep performance     |

---

## Customisation

All data is hardcoded in `index.html` for demo purposes. To adapt for a real client:

- Replace contact/company/deal data with live CRM data via API calls
- Connect modals to a backend (Node.js, Supabase, Firebase, etc.)
- Add authentication before the dashboard loads
- Extend the pipeline columns to match the client's actual sales stages

---

## Built by

**Thari Tech** — Technology solutions for modern businesses.

> Demo CRM built and designed by [Unam-spec](https://github.com/Unam-spec)
