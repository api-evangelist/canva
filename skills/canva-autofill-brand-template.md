---
name: canva-autofill-brand-template
description: Create a Canva design by autofilling a brand template's data fields through the REST API.
api: openapi/canva-autofill-api-openapi.yml
operations:
  - listBrandTemplates
  - getBrandTemplateDataset
  - createDesignAutofillJob
  - getDesignAutofillJob
generated: '2026-10-20'
method: generated
---
# Autofill a brand template

Server: `https://api.canva.com/rest`. Autofill needs scope `design:content:write`, and brand templates need `brandtemplate:meta:read` / `brandtemplate:content:read`. Brand templates and autofill need a Canva plan that includes them; check `getUserCapabilities` first (conventions: capabilities_precheck).

1. `listBrandTemplates` (GET /v1/brand-templates) — search with `query`, page with `continuation`, and narrow to templates that have fields using `dataset`.
2. `getBrandTemplateDataset` (GET /v1/brand-templates/{brandTemplateId}/dataset) — read the field names and their types (text, image, chart).
3. `createDesignAutofillJob` (POST /v1/autofills) — send the brand template id and a `data` value for each field. Image fields take asset ids, so upload images first (see canva-upload-asset-from-url).
4. `getDesignAutofillJob` (GET /v1/autofills/{jobId}) — poll until `success`, which returns the new design, or `failed`.

Rules:
- Each job makes one design, so for bulk work run one job per row. Respect the 100 requests/minute per-user limit on the read operations.
- There is no idempotency key. Keep track of which rows already produced a design before you retry.
- MCP equivalents: `search-brand-templates`, `get-brand-template-dataset`, `autofill-design`. Canva also publishes a bulk-create skill: skills/canva-claude-skills/skills/bulk-create/SKILL.md.
