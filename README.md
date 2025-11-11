# 🧭 Eckohaus Orchestration Pilot

_© 2025 Eckohaus Ltd — Internal Research & Development Repository_  
_This repository underpins the automated compliance orchestration system integrating Eckohaus Ltd’s UK filings (Companies House, HMRC) with internal workflow automation._

---

## 🧩 Overview

The **Eckohaus Orchestration Pilot** is an internal proof-of-concept that connects Companies House data with automated audit trails and reminder systems.

It operates across **test**, **live**, and **weekly** workflows, using GitHub Actions to:
- Query Companies House APIs
- Archive and version responses as JSON
- Append entries to a persistent orchestration ledger
- Prepare for future event-sequenced automation (accounts & confirmation filings)

---

## 📂 Repository Layout (as of October 2025)
```
Eckohaus-Orchestration-Pilot/
│
├── README.md
│   → Main project overview and licence notice.
│
├── orchestration-ledger.md
│   → Event-sequenced compliance log (pre-filing, filing, post-filing).
│
├── CHANGELOG.md
│   → Versioned changelog following Keep a Changelog 1.1.0.
│
├── .github/
│   └── workflows/
│       ├── compliance-check.yml
│       ├── compliance-check-live.yml
│       └── compliance-check-weekly.yml
│       → Automated workflows for Companies House data checks.
│
├── config/
│   └── metadata.yml
│   → Company and jurisdictional metadata (UK ↔ Indonesia).
│
├── data/
│   ├── responses/
│   └── sandbox_responses/
│   → Archived Companies House JSON responses (live & test).
│
└── scripts/
    ├── README.md
    └── analyze_workflow_logs.py
    → Workflow log analysis and repository structure integration.
```
---

## ⚙️ Current Workflows

| Workflow | Purpose | Status |
|-----------|----------|--------|
| `compliance-check.yml` | Sandbox test workflow for CH API validation | ✅ Active |
| `compliance-check-live.yml` | Live CH data retrieval & audit logging | 🧩 In propagation stage |
| `compliance-check-weekly.yml` | Scheduled production cycle (Mon 10:00 UTC) | ⏸ Development phase |

Each workflow interacts with `config/metadata.yml` for company details and API environment parameters.  
Live responses are archived in `/data/responses/` and recorded in `orchestration-ledger.md`.

---

## 📊 Workflow Log Analysis

The repository includes a Python-based log analyzer that performs line-by-line analysis of GitHub Actions workflow logs, integrating them with the repository folder and file structure.

**Key Features**:
- Line-by-line parsing of workflow execution logs
- Integration with repository structure (`config/`, `data/`, `.github/workflows/`)
- Error and warning detection
- API call tracking (Companies House)
- File operation monitoring
- Security findings analysis (CodeQL)
- Automated markdown report generation

**Usage**:
```bash
python3 scripts/analyze_workflow_logs.py
```

See `scripts/README.md` for detailed documentation.

---

## 🪶 Co-author Traceability  
```
Co-authored-by: system operator <wanda@openai.com>
Co-authored-by: system administrator  <info@eckohaus.co.uk>
```
---

### 📜 Licence
This project is maintained under the **Eckohaus Ltd Private Use Licence**.  
Reproduction or external redistribution is not permitted without written consent.  

For further enquiries: [info@eckohaus.co.uk](mailto:info@eckohaus.co.uk)

---

_Last synchronised via GitHub Actions — October 2025_
