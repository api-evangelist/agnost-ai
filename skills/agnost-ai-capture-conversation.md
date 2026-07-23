---
name: Capture an agent conversation into Agnost
description: Send a production AI agent conversation (session + turn/tool events) to Agnost AI for monitoring and analytics.
api: openapi/agnost-ai-openapi-original.yml
operations: [captureSession, captureEvent]
generated: '2026-07-18'
method: generated
---

# Capture an agent conversation into Agnost

Instrument a chat/voice agent so each conversation and its turns land in the
Agnost dashboard. Prefer the official SDKs (`agnost`, `agnostai`, `agnost-mcp`)
in application code; use these raw operations only for custom ingestion.

## Auth
- Ingestion is routed by your organization UUID in the `x-org-id` header.
- The org ID is a **public routing identifier**, not a secret. It does not grant
  dashboard read access.
- Base URL: `https://api.agnost.ai` (or send OTLP traces to
  `https://otel.agnost.ai/v1/traces` with header `X-Agnost-Org-ID`).

## Steps
1. **Start the session** at the beginning of a conversation — `captureSession`
   (`POST /api/v1/capture-session`). Provide a stable `session_id` and a
   pseudonymous `user_data.user_id` (never a raw email/name — see data
   governance).
2. **Record each turn or tool call** — `captureEvent`
   (`POST /api/v1/capture-event`). Send one turn-pair (user input + agent
   output) or one tool call per event, with `event_id` and the same
   `session_id`.
3. Verify in the dashboard **Raw logs** that the event shows the expected org
   ID, user ID, session ID, and agent/tool name.

## Rules
- Redact/pseudonymize PII before sending; Agnost does not auto-redact.
- Errors return `{"error":"<message>"}` with HTTP 400 on missing/invalid fields
  (validate `session_id`, `event_id`, `user_data.user_id`). See
  `errors/agnost-ai-problem-types.yml`.
- No idempotency key is supported; use a unique `event_id` per event to avoid
  duplicates.
