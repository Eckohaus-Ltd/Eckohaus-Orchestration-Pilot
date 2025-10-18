# Eckohaus Orchestration Pilot

A pilot repository demonstrating the orchestration of corporate compliance events for **Eckohaus Ltd** using the **Companies House API**.  
The project structures filings, reminders, and verification steps as an **event-sequenced ledger**, forming a prototype for dual-jurisdiction workflows (UK ↔ Indonesia).

## Overview

This repository models how corporate administrative events—such as accounts filings and confirmation statements—can be represented as a time-ordered sequence.  
It serves as a private R&D environment for refining orchestration logic before potential adaptation to other jurisdictions, including the Indonesian OSS/AHU systems.

## Repository layout (as of October 2025)

```plaintext
Eckohaus-Orchestration-Pilot/
│
├── README.md
│   → Main project overview and licence notice.
│
├── orchestration-ledger.md
│   → Event-sequenced compliance log (pre-filing, filing, post-filing).
│
├── .github/
│   └── workflows/
│       └── compliance-check.yml
│       → Workflow stub for Companies House API status checks.
│
├── config/
│   └── metadata.yml
│   → Company and jurisdictional metadata (UK ↔ Indonesia).
│
└── data/
    └── sample_companyhouse.json
    → Placeholder dataset for Companies House API responses.
```

## Status

Private internal research project under active development.  
No public distribution, automation, or integration outside Eckohaus Ltd is authorised at this stage.

---

_© 2025 Eckohaus Ltd. All rights reserved._  
_This repository and its contents are maintained under the **Private Use Licence** (see `LICENSE.md`)._
