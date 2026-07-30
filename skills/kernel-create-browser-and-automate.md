---
name: Create a cloud browser and automate it with Playwright
description: Spin up a Kernel cloud Chromium session, drive it with Playwright/TypeScript, capture a screenshot, then tear it down.
api: openapi/kernel-openapi-original.yml
operations: [postBrowsers, executePlaywrightCode, takeScreenshot, deleteBrowsersByIdOrName]
---

# Create a cloud browser and automate it with Playwright

Use this to run headless/headful browser automation on Kernel's cloud without managing your own Chromium infrastructure.

## Auth
All calls use `Authorization: Bearer <KERNEL_API_KEY>`. Keys are org- or project-scoped; set `KERNEL_PROJECT` to scope a request (see `conventions/kernel-conventions.yml`).

## Steps
1. **Create a browser session** — `postBrowsers` (`POST /browsers`). Optionally pass `profile_id`, `proxy_id`, `start_url`, and telemetry config. Save the returned browser `id`.
2. **Run automation** — `executePlaywrightCode` (`POST /browsers/{id}/playwright/execute`) with your Playwright/TypeScript snippet against the live session.
3. **Capture a screenshot** — `takeScreenshot` (`POST /browsers/{id}/computer/screenshot`) to grab the current viewport.
4. **Clean up** — `deleteBrowsersByIdOrName` (`DELETE /browsers/{id_or_name}`) to end the session and stop billing. Idle sessions can also enter Standby Mode.

## Conventions & errors
- Resources are addressable by `{id_or_name}`.
- No idempotency-key contract — do not blind-retry `postBrowsers` on timeout; list/reconcile first.
- Handle `429` with `Retry-After` backoff; `404` means the session id/name is gone; error envelope is `{code, message, details[]}` (see `errors/kernel-problem-types.yml`).
