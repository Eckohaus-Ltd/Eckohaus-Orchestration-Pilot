# 🧾 Eckohaus Orchestration Pilot — Changelog

_All notable changes to this project will be documented in this file._  
_This changelog follows the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) convention._  
_Semantic versioning: MAJOR.MINOR.PATCH_

---

## [1.1.0] — 2025-10-19
### Added
- Introduced `orchestration-ledger.md` for live audit tracking and compliance event documentation.
- Implemented `compliance-check-live.yml` with weekday-aware retry logic for Companies House 404 propagation.
- Added `config/metadata.yml` refinements (jurisdiction, environment, and maintainer fields).
- Began structured storage of Companies House responses in `/data/responses/` and `/data/sandbox_responses/`.

### Improved
- Enhanced workflow logging with clear CH API query states and timestamps.
- Updated standard co-author attribution footer for all extended commit descriptions.
- Improved formatting consistency across documentation files (`README.md`, `orchestration-ledger.md`).

### Fixed
- Resolved metadata parsing in live/sandbox workflows (removed redundant quote characters).

### Notes
- Awaiting first verified Companies House live response following API propagation.
- Weekly automation schedule temporarily disabled during development.
- Next milestone: enable `compliance-check-weekly.yml` for stable production cycles.

---

## [1.0.0] — 2025-10-18
### Initialisation
- Created repository structure and base workflows.
- Set up sandbox Companies House API test integration.
- Added initial metadata and private-use licensing model.
- Defined core repository documentation (`README.md`, `LICENSE.md`).

---

### 🪶 Co-author Traceability  
```
Co-authored-by: system operator <wanda@openai.com>  
Co-authored-by: system administrator <Corvin Nehal Dhali> <info@eckohaus.co.uk>
```

---

## [2025-10-20] — 🛰️ Live API Orchestration Verified
**Summary:**  
First successful live run of the Companies House compliance workflow for  
Eckohaus Ltd (Company No. 15451433).

### 🧩 Details
- Live API key authenticated successfully (`CH_API_KEY_LIVE`)
- Response archived at `data/responses/response_live_20251020_0320.json`
- Ledger auto-updated and committed (`commit 1f814c1`)
- Workflow parity confirmed with sandbox configuration

---

### 🪶 Co-author Traceability  
```
Co-authored-by: system operator <wanda@openai.com>  
Co-authored-by: system administrator <Corvin Nehal Dhali> <info@eckohaus.co.uk>
```

---

© 2025 Eckohaus Ltd — Internal Orchestration Record  
_This changelog is automatically referenced by the Eckohaus Orchestration Pilot documentation suite._
