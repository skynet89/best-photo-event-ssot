# AI Development Guidelines

This project is multi-AI developed.

Rules:

1. Always reference /contracts as single source of truth.
2. Never rename API endpoints defined in OpenAPI.
3. Do not change JSON schema fields.
4. All breaking changes require v2 contracts.
5. Edge and Cloud implementations must be compatible.

AI prompts must include:
- OpenAPI contracts
- License schema
- Checkin schema
