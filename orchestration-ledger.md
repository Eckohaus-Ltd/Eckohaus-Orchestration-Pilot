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

## Next Steps
- Finalise live API key authentication.
- Extend workflow to parse JSON and surface next filing deadlines.
- Integrate reminder scheduling into GitHub Actions or external cron system.

---

_Maintained internally under the [Private Use Licence](./LICENSE.md)._  
_Contact: info@eckohaus.blog_
