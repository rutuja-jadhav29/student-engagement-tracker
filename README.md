# Student Engagement & Outcomes Tracker
**Tool:** Airtable | **Type:** Personal Portfolio Project | **Year:** 2026

A end-to-end student data tracking system simulating the data infrastructure used by higher education programs to monitor engagement, persistence, and learning outcomes across multiple cohorts.

---

## Project Overview

This project replicates the kind of data system used by college success, experiential learning, or student affairs programs — built entirely in Airtable with synthetic data representing 150 students across 2 cohort years and 3 learning pathways.

**The system answers 4 core program questions:**
- Which students are at risk of withdrawing?
- How are outcomes changing year over year?
- Are students improving on pre/post assessments?
- Which learning pathways are growing in demand?

---

## What Was Built

### 3 Linked Tables
| Table | Records | Purpose |
|---|---|---|
| Students | 150 | Demographics, enrollment status, pathway, survey scores |
| Sessions | 102 | Program touchpoints, attendance, modality, topics |
| Survey Responses | 280 | Pre/post Likert scores across self-efficacy, belonging, career clarity |

### 4 Analytical Views
- **At-risk students** — filters students with fewer than 3 sessions attended for early outreach
- **Cohort Comparison** — groups students by year and pathway to surface year-over-year trends
- **Session Calendar** — maps all 102 program sessions chronologically by date
- **Pre vs. Post Tracker** — groups survey responses by student to show score change over time

### Live Dashboard
- Total student count (150)
- Cohort growth bar chart (2023 vs 2024)
- Enrollment status pivot table (Active / Withdrawn / Graduated by year)

---

## Key Findings

- **34% cohort growth** from 2023 (64 students) to 2024 (86 students), signaling increased program demand
- **2023 retention breakdown:** 37 Active · 15 Withdrawn · 12 Graduated
- **2024 retention breakdown:** 53 Active · 18 Withdrawn · 15 Graduated
- Pre/post survey data across 280 responses shows measurable gains in self-efficacy and career clarity, providing evidence of program effectiveness


<img width="1321" height="562" alt="Screenshot 2026-06-11 at 12 57 57 PM" src="https://github.com/user-attachments/assets/1262b011-e684-4bfc-966c-3e1c6c4e69ac" />



<img width="1328" height="637" alt="Screenshot 2026-06-11 at 12 57 43 PM" src="https://github.com/user-attachments/assets/86394be6-019a-405a-9ded-78e76b17ca6e" />




<img width="1314" height="553" alt="Screenshot 2026-06-11 at 12 58 13 PM" src="https://github.com/user-attachments/assets/df37a0cd-f154-4e40-9d76-03c6ff491531" />

---

## Data Dictionary

| Field | Table | Type | Description |
|---|---|---|---|
| Student ID | Students | Text | Unique identifier (STU0001–STU0150) |
| Cohort Year | Students | Single select | 2023 or 2024 |
| Enrollment Status | Students | Single select | Active / Withdrawn / Graduated |
| Learning Pathway | Students | Single select | Career Readiness / Academic Success / Leadership Development |
| Demographics | Students | Multi-select | First-gen, Pell-eligible, or both |
| Sessions Attended | Students | Number | Total program touchpoints attended |
| Pre/Post Survey Score | Students | Number | Composite Likert score (1–5 scale) |
| Score Change | Students | Number | Post minus Pre score |
| Session Date | Sessions | Date | Date of program event |
| Modality | Sessions | Single select | In-person / Virtual / Hybrid |
| Survey Type | Survey Responses | Single select | Pre / Post / Follow-up |
| Composite Score | Survey Responses | Number | Average of Q1–Q3 Likert items |

---

## Files in This Repository

```
├── students.csv              # 150 student records with demographics and outcomes
├── sessions.csv              # 102 program session records
├── survey_responses.csv      # 280 pre/post survey response records
└── README.md                 # Project documentation
```

---

## Tools Used
- **Airtable** — database design, linked tables, views, dashboard
- **Python** — synthetic data generation
- **CSV** — data import and portability

---

## Relevance to Higher Education Data Roles

This project directly demonstrates:
- Building and maintaining trackers in Airtable
- Collecting and structuring quantitative data on student demographics, engagement, and outcomes
- Synthesizing multi-year data to identify patterns (cohort growth, retention rates)
- Supporting pre/post assessment tracking across learning pathways
- Producing dashboard visualizations for internal stakeholders
- Documenting data structure for transferable, sustainable systems

---

## Live Airtable Base
[View the live tracker →](#) *https://airtable.com/invite/l?inviteId=invRHXmBScwPx5izO&inviteToken=246f9201f97705456641d00170c2be47e4e570349bf919f39a8222ca7faa3bd1&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts*
