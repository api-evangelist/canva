---
name: canva-upload-asset-from-url
description: Upload an image or video into a user's Canva library from a public URL, then read the resulting asset.
api: openapi/canva-asset-api-openapi.yml
operations:
  - createUrlAssetUploadJob
  - getUrlAssetUploadJob
  - getAsset
generated: '2026-10-20'
method: generated
---
# Upload an asset from a URL

Server: `https://api.canva.com/rest`. Needs scope `asset:write` to upload and `asset:read` to read.

1. `createUrlAssetUploadJob` (POST /v1/url-asset-uploads) — send the asset name and a publicly reachable URL. The response is a job with `status: in_progress`.
2. `getUrlAssetUploadJob` (GET /v1/url-asset-uploads/{jobId}) — poll with backoff until `success` (the asset is inline) or `failed`.
3. `getAsset` (GET /v1/assets/{assetId}) — read the asset's metadata and thumbnail. Rate limit: 100 requests/minute per user.

Rules:
- There is no idempotency key. A retried create can upload a duplicate asset.
- To send a binary instead of a URL, use `CreateAssetUploadJob` / `GetAssetUploadJob` (POST /v1/asset-uploads).
- MCP equivalent: the documented `upload-asset-from-url` tool.
