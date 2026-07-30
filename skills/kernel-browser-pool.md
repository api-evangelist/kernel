---
name: Acquire and release browsers from a pre-warmed pool
description: Create a browser pool, acquire a warm browser for low-latency work, release it back, and flush idle browsers.
api: openapi/kernel-openapi-original.yml
operations: [postBrowserPools, acquireFromBrowserPoolByIdOrName, releaseToBrowserPoolByIdOrName, flushBrowserPoolByIdOrName]
---

# Acquire and release browsers from a pre-warmed pool

Use this when you need sub-second browser starts by reusing pre-warmed sessions instead of cold-creating each time.

## Auth
`Authorization: Bearer <KERNEL_API_KEY>`.

## Steps
1. **Create a pool** — `postBrowserPools` (`POST /browser_pools`) with size, `fill_rate_per_minute`, optional `profile`, and standby settings; save the pool `id_or_name`.
2. **Acquire a browser** — `acquireFromBrowserPoolByIdOrName` (`POST /browser_pools/{id_or_name}/acquire`) to check out a warm session; use its browser `id` for automation.
3. **Release it back** — `releaseToBrowserPoolByIdOrName` (`POST /browser_pools/{id_or_name}/release`) when done so the session is recycled.
4. **Flush idle** — `flushBrowserPoolByIdOrName` (`POST /browser_pools/{id_or_name}/flush`) to drop idle browsers.

## Conventions & errors
- Reserved pool capacity counts toward your org concurrency limit whether or not browsers are acquired.
- Pools support auto-standby (suspend when idle, resume on request).
- Handle `429`/`Retry-After`; `409` may indicate the pool is at capacity.
