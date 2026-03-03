# Best Photo Event - Architecture v1 (SSOT)

This repository is the Single Source of Truth (SSOT) for:
- Contracts (OpenAPI + JSON Schemas)
- Folder layout for Edge
- Product plans and operational rules

Contract-first policy:
- v1 contracts MUST NOT be changed.
- Any changes require v2 contracts in /contracts/v2/ and updated spec.

Key invariants:
- Edge runs offline-first on Linux with local Postgres + Redis.
- Kiosk clients only see watermarked previews.
- Originals are never exposed publicly.
- Printing default is hotfolder (no direct CUPS printing in v1).
- Licensing is vendor-signed Ed25519 JSON; edge validates offline.
