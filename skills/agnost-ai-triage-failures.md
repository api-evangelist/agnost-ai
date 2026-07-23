---
name: Triage agent failures in Agnost
description: Query the Agnost dashboard to find the highest-impact agent failures, frustrated conversations, and SOP violations, then drill into examples.
api: openapi/agnost-ai-openapi-original.yml
operations: [getErrors, getToolErrorDistribution, getSOPViolations, summarizeIntentDistribution, spotlightSearch, getConversationDetail]
generated: '2026-07-18'
method: generated
---

# Triage agent failures in Agnost

Find what is breaking in a production agent and pull concrete examples. This is
the same surface the hosted MCP server (`https://mcp.agnost.ai/mcp`) exposes in
natural language.

## Auth
- Dashboard endpoints require `Authorization: Bearer <jwt>` **or** `x-api-key`
  (`agnost_<64-hex>`), plus the right `x-org-id`.
- Base URL: `https://api.agnost.ai`.
- Most analytics endpoints are `POST` with a JSON body carrying a `TimeRange`
  (start/end) and optional `QueryFilters`.

## Steps
1. **Surface errors** — `getErrors` (`POST /dashboard/api/errors`) for the time
   window; use `getToolErrorDistribution`
   (`POST /dashboard/api/tool-error-distribution`) to see which tools fail most.
2. **Check SOP violations** — `getSOPViolations`
   (`POST /dashboard/api/sop-violations`) to find where the agent broke a
   Standard Operating Procedure.
3. **Read intent signal** — `summarizeIntentDistribution`
   (`POST /dashboard/api/summarize-intent-distribution`) to see the dominant
   user intents and where they cluster with frustration.
4. **Find examples** — `spotlightSearch`
   (`POST /dashboard/api/spotlight-search`) with a natural-language/filter query
   to locate matching conversations.
5. **Drill in** — `getConversationDetail`
   (`POST /dashboard/api/conversation-detail`) to read the full failing
   conversation before proposing a fix.

## Rules
- Scope every call to the correct `x-org-id`; 401/403 means missing/incorrect
  credential or org scope (see `errors/agnost-ai-problem-types.yml`).
- Pagination is page-based (`page`, `page_size`); no cursors.
- Read-only triage — none of these operations mutate agent data.
