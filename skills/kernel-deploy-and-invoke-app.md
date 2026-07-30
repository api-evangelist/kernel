---
name: Deploy a Kernel app and invoke an action
description: Create a deployment, invoke one of its actions, then poll or stream the invocation to completion.
api: openapi/kernel-openapi-original.yml
operations: [postDeployments, postInvocations, getInvocationsById, getInvocationsEventsById]
---

# Deploy a Kernel app and invoke an action

Use this to run serverless agent/automation code on Kernel's App platform.

## Auth
`Authorization: Bearer <KERNEL_API_KEY>`.

## Steps
1. **Create a deployment** — `postDeployments` (`POST /deployments`) for your app; save the deployment `id` and watch build status via `getDeploymentsEventsById` (SSE).
2. **Invoke an action** — `postInvocations` (`POST /invocations`) with the app/action name and a JSON `payload`; save the invocation `id`.
3. **Stream progress** — `getInvocationsEventsById` (`GET /invocations/{id}/events`, SSE) to follow the run in real time.
4. **Read the result** — `getInvocationsById` (`GET /invocations/{id}`) for the final status/output.

## Conventions & errors
- CLI equivalent: `kernel deploy index.ts` then `kernel invoke my-app action-name --payload '{...}'`.
- Invocations may spawn browsers (`getInvocationsBrowsersById`).
- Error envelope is `{code, message, details[]}`; handle `429`/`Retry-After` and `409` conflicts on redeploy.
