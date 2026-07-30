---
name: Log a browser into a site with Managed Auth
description: Create a managed-auth connection, start a login flow, submit field values, and watch the flow complete over SSE.
api: openapi/kernel-openapi-original.yml
operations: [postAuthConnections, postAuthConnectionsLogin, postAuthConnectionsSubmit, getAuthConnectionsEventsById]
---

# Log a browser into a site with Managed Auth

Use this to have Kernel authenticate a browser session into a third-party site and keep the session healthy.

## Auth
`Authorization: Bearer <KERNEL_API_KEY>`.

## Steps
1. **Create the connection** — `postAuthConnections` (`POST /auth/connections`) targeting the site/profile; save the connection `id`.
2. **Start login** — `postAuthConnectionsLogin` (`POST /auth/connections/{id}/login`) to begin the flow.
3. **Stream events** — `getAuthConnectionsEventsById` (`GET /auth/connections/{id}/events`, SSE) to observe required fields, MFA prompts, and status transitions.
4. **Submit field values** — `postAuthConnectionsSubmit` (`POST /auth/connections/{id}/submit`) whenever the event stream requests credentials or an MFA/TOTP code. Stored credentials can come from a `CredentialProvider` (e.g. 1Password).

## Conventions & errors
- Events stream as `text/event-stream` (SSE), not webhooks.
- Sessions are re-authenticated automatically by Kernel; most stay valid for days.
- On `401`/`403` re-check the API key and project scope; on `429` back off using `Retry-After`.
