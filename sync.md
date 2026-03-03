# Edge -> Cloud Sync v1

Cloud base URL:
https://saas-photoapp.digitalsupport.eu

Edge must:
- Register with provisioning token: POST /api/edges/register
- Send periodic check-ins: POST /api/edges/checkin

Check-in payload must match contracts/checkin-schema.v1.json
and must be signed with Edge Ed25519 private key.

Idempotency:
- Use seq monotonic increasing
- Cloud stores last_seq per edge and rejects duplicates/out-of-order
