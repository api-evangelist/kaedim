---
name: Generate a 3D asset from images with Kaedim
description: Register a webhook, submit images for AI 2D-to-3D generation, and retrieve the finished models.
api: openapi/kaedim-web-api-openapi.yml
operations: [registerHook, processImage, fetchRequest, refreshJWT]
---

# Generate a 3D asset with Kaedim

Kaedim converts 2D images (photos, sketches, concept art) into 3D models. The API
is Enterprise-only, authenticated with an `X-API-Key` header plus a JWT bearer
token, and generation is asynchronous (typically 10-15 minutes).

## Prerequisites
- An Enterprise `X-API-Key` (Settings > API Keys in the Kaedim app).
- Your `devID` (user settings page).
- An HTTPS endpoint to receive webhook callbacks.
- Base URL: `https://api.kaedim3d.com/api/v1`

## Steps

1. **Register your webhook** — `registerHook` (POST `/registerHook`). Send
   `X-API-Key` + JSON body `{ devID, destination }` where `destination` is your
   HTTPS endpoint. The 201 response returns the `jwt` you use to authorize the
   next calls.

2. **Submit images** — `processImage` (POST `/process`, multipart/form-data).
   Send `X-API-Key` + `Authorization: Bearer {jwt}`. Include `devID`, `LoQ`
   (`standard` | `high` | `ultra`), and either `imageUrls` or `images` (up to 6,
   5MB each). Optional: `polycount`, `height`/`width`/`depth`, `projectID`. Set
   `test: true` to run without consuming credits. Capture the returned
   `requestID`.

3. **Receive the result** — Kaedim POSTs a signed webhook to your `destination`
   when the asset completes. Verify the `kaedim-signature` header (HMAC-SHA256
   of timestamp + UTF-8 JSON payload, keyed with your secret, timing-safe
   compare). The payload's `completedModels` carries download URLs for fbx, glb,
   mtl, obj, usd, gltf.

4. **Or poll** — `fetchRequest` (GET `/fetchRequest?devID=...&requestID=...`)
   returns the request with its `iterations[]` model URLs.

## Rules
- **JWT expires after 12 hours** — refresh with `refreshJWT` (POST `/refreshJWT`,
  `refresh-token` header + `{ devID }` body) rather than re-registering.
- **Download links expire after 1 hour** — fetch and store models promptly.
- No idempotency key: track work by the returned `requestID`, do not blindly retry `/process`.
- Errors are HTTP status + `{ status, message }` (400 bad payload, 404 unknown user, 406 invalid LoQ).
