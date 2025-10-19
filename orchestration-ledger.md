# Eckohaus Orchestration Ledger

_© 2025 Eckohaus Ltd. Internal Research & Development Record_

This document serves as a human-readable event log for the **Eckohaus Orchestration Pilot**,  
tracking key milestones, workflow runs, and compliance events across the Companies House API integration.

---

## Ledger Overview

Each entry below corresponds to a structured orchestration event.  
These may include:
- **Pre-filing** checks (e.g. account due dates, confirmation statements)
- **Filing** events (submissions or reminders)
- **Post-filing** validations and reconciliations

---

## Event Log

| Date (UTC) | Event Type | Description | Notes |
|-------------|-------------|-------------|-------|
| 2025-10-19 | Initialisation | Created project structure and metadata. | Repository and workflows established for test & live API. |
| 2025-10-19 | API Test | Successful sandbox workflow run. | Returned “Resource not found” as expected (mock test). |
| 2025-10-19 | API Live | First live Companies House query. | Returned “Invalid Authorization” (key verification stage). |

---

## Pending Orchestration Schedule

| Target Period | Scope | Notes |
|----------------|--------|-------|
| December 2025 | Pre-filing cycle | Initial live data pull and status check before January 2026 deadlines. |
| Q1 2026 | Filing + confirmation events | To synchronise Companies House filings with HMRC PAYE and pension reconciliations. |
| Mid-2026 | API integration review | Assess Companies House → internal ledger consistency for future automation. |

---

_All future schedule events are provisional until verified against Companies House and HMRC confirmation dates._

---

_Maintained internally under the [Private Use Licence](./LICENSE.md)._  
_Contact: info@eckohaus.blog_
