# BA Portfolio Project: Vendor Data Onboarding & Integration Process

**A fictional case study by Dwij Siyal, Business Analyst**

> This project is modeled loosely on real business analysis experience gained while working on Virtual Visit, Telehealth, and Remote Patient Monitoring programs at a Canadian provincial health authority. The organization ("Prairie Telehealth Network"), vendors, and all data shown in this repository are entirely fictional and contain no proprietary information.

📄 **[Read the full combined portfolio (PDF)](BA-Portfolio-Vendor-Onboarding/07-Final-Portfolio/BA-Portfolio-Dwij-Siyal.pdf)**

---

## The Problem

Prairie Telehealth Network (PTN) contracts with third-party vendors to deliver Virtual Visit, Telehealth, and Remote Patient Monitoring (RPM) services. Each vendor submits usage and clinical data in its own internally standardized format — but no standardized *summary layer* exists across vendors. Each month, the Analytics & Reporting team manually reconciles three structurally different datasets to produce Ministry of Health performance reports, a process that takes **6–8 business days** and is prone to error.

This project designs a standardized vendor onboarding process built on a two-tier model:
- A **standardized monthly summary schema** for consistent external (Ministry of Health) reporting
- **Structured vendor detail data** retained for internal, service-specific dashboards

## What's in This Repo

| Phase | Deliverable | Description |
|---|---|---|
| 1 | [Project Brief](BA-Portfolio-Vendor-Onboarding/01-Project-Brief) | Problem definition, scope, objectives, and success criteria |
| 2 | [Current State Process Map](BA-Portfolio-Vendor-Onboarding/02-Current-State-Process-Map) | Swimlane diagram of the manual reconciliation process and its pain points |
| 3 | [Stakeholder Analysis](BA-Portfolio-Vendor-Onboarding/03-Stakeholder-Analysis) | Power/Interest Matrix and RACI Chart |
| 4 | [Requirements Document](BA-Portfolio-Vendor-Onboarding/04-Requirements) | Business, Functional, and Non-Functional requirements (MoSCoW-prioritized, fully traced to business needs) |
| 5 | [Data Mapping Table](BA-Portfolio-Vendor-Onboarding/05-Data-Mapping) | Field-level mapping of 3 fictional vendors to a standardized summary schema |
| 6 | [Future State Process Map](BA-Portfolio-Vendor-Onboarding/06-Future-State-Process-Map) | Redesigned process showing how each current-state pain point is resolved |
| 7 | [Final Portfolio](BA-Portfolio-Vendor-Onboarding/07-Final-Portfolio) | All phases combined into a single PDF |

## Highlights Worth Noting

- **The data mapping isn't a clean 1-to-1 exercise.** The three fictional vendors have genuinely different data shapes — one session-based, one encounter-based, one reading-based (RPM) — so several target fields are intentionally left `N/A` for vendors where they don't apply (e.g., a reading-based vendor has no "session duration"). Forcing every field to map for every vendor would have meant fabricating data.
- **Two semantic mismatches are explicitly flagged**, not silently blended: RPM's "issue count" reflects clinical alerts, not technical issues, and its "total events" counts device readings, not sessions. These distinctions are documented so they don't get lost in aggregate reporting.
- **The current state and future state process maps use the same visual language** (red = pain point, green = resolved), so the two diagrams can be read side by side as a before/after.

## Tools Used
Microsoft Word & Excel, Lucidchart, fictional data modeling

## Structure
```
├── 01-Project-Brief/
├── 02-Current-State-Process-Map/
├── 03-Stakeholder-Analysis/
├── 04-Requirements/
├── 05-Data-Mapping/
├── 06-Future-State-Process-Map/
└── 07-Final-Portfolio/
    └── BA-Portfolio-Dwij-Siyal.pdf
```

---

📫 Connect with me: [LinkedIn](https://www.linkedin.com/in/dwij-siyal-9b98a61a1/)
