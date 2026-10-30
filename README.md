# Kernel

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kernel is browser infrastructure for AI agents and automations. It runs sandboxed cloud Chromium browsers that spin up in under 30ms, with Playwright execution, computer-use controls, managed authentication into third-party sites, reusable browser profiles, proxies, pre-warmed browser pools, session replays, live telemetry, and a serverless App platform for deploying and invoking agent actions. Kernel exposes a REST API (OpenAPI 3.1, 135 operations across 22 tags), first-party TypeScript, Python and Go SDKs, a CLI, and a centrally hosted MCP server so agents can drive real browsers. Backed by General Catalyst.

**Areas:** Company · Browser Automation · Web Agents · Browser Infrastructure · AI Agents · Playwright · Cloud Browser · Computer Use · MCP · Managed Auth

## Kernel on APIs.io

Everything profiled for Kernel is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kernel/](https://apis.io/providers/kernel/)** — or go straight to one of the APIs or properties below.

### APIs (22)

- [Kernel API Keys API](https://apis.io/apis/kernel/kernel-api-keys-api/) — Create and manage API keys for organization and project-scoped access.
- [Kernel Apps API](https://apis.io/apis/kernel/kernel-apps-api/) — List applications and versions.
- [Kernel Audit Logs API](https://apis.io/apis/kernel/kernel-audit-logs-api/) — Read audit log records for the authenticated organization.
- [Kernel Browser Computer Controls API](https://apis.io/apis/kernel/kernel-browser-computer-controls-api/) — Control mouse, keyboard, and screen on the browser instance.
- [Kernel Browser Filesystem API](https://apis.io/apis/kernel/kernel-browser-filesystem-api/) — Read, write, and manage files on the browser instance.
- [Kernel Browser Logs API](https://apis.io/apis/kernel/kernel-browser-logs-api/) — Stream logs from the browser instance.
- [Kernel Browser Playwright API](https://apis.io/apis/kernel/kernel-browser-playwright-api/) — Execute Playwright code against the browser instance.
- [Kernel Browser Pools API](https://apis.io/apis/kernel/kernel-browser-pools-api/) — Create and manage browser pools for acquiring and releasing browsers.
- [Kernel Browser Processes API](https://apis.io/apis/kernel/kernel-browser-processes-api/) — Execute and manage processes on the browser instance.
- [Kernel Browser Replays API](https://apis.io/apis/kernel/kernel-browser-replays-api/) — Record and manage browser session video replays.
- [Kernel Browser Telemetry API](https://apis.io/apis/kernel/kernel-browser-telemetry-api/) — Stream live telemetry events from a browser session.
- [Kernel Browsers API](https://apis.io/apis/kernel/kernel-browsers-api/) — Create and manage browser sessions.
- [Kernel Credential Providers API](https://apis.io/apis/kernel/kernel-credential-providers-api/) — Configure external credential providers like 1Password.
- [Kernel Credentials API](https://apis.io/apis/kernel/kernel-credentials-api/) — Create and manage credentials for authentication.
- [Kernel Deployments API](https://apis.io/apis/kernel/kernel-deployments-api/) — Create and manage app deployments and stream deployment events.
- [Kernel Extensions API](https://apis.io/apis/kernel/kernel-extensions-api/) — Create, list, retrieve, and delete browser extensions.
- [Kernel Invocations API](https://apis.io/apis/kernel/kernel-invocations-api/) — Invoke actions and stream or query invocation status and events.
- [Kernel Managed Auth API](https://apis.io/apis/kernel/kernel-managed-auth-api/) — Create and manage auth connections for automated credential capture and login.
- [Kernel Organization API](https://apis.io/apis/kernel/kernel-organization-api/) — Read and manage organization-level limits.
- [Kernel Profiles API](https://apis.io/apis/kernel/kernel-profiles-api/) — Create, list, retrieve, and delete browser profiles.
- [Kernel Projects API](https://apis.io/apis/kernel/kernel-projects-api/) — Create and manage projects for resource isolation within an organization.
- [Kernel Proxies API](https://apis.io/apis/kernel/kernel-proxies-api/) — Create and manage proxy configurations for routing browser traffic.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [Kernel - create a browser, run Playwright, screenshot, tear down](https://apis.io/arazzos/kernel/kernel-browser-automate/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [kernel](https://apis.io/servers/kernel/kernel/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Kernel Agentic Access](https://apis.io/agentic-access/kernel/kernel-agentic-access/)

#### Collections (22)

Postman and Open Collection request collections.

- [Kernel API Keys API](https://apis.io/collections/kernel/open-kernel-api-keys-api/)
- [Kernel API Keys Apps API](https://apis.io/collections/kernel/open-kernel-apps-api/)
- [Kernel API Keys Audit Logs API](https://apis.io/collections/kernel/open-kernel-audit-logs-api/)
- [Kernel API Keys Browser Computer Controls API](https://apis.io/collections/kernel/open-kernel-browser-computer-controls-api/)
- [Kernel API Keys Browser Filesystem API](https://apis.io/collections/kernel/open-kernel-browser-filesystem-api/)
- [Kernel API Keys Browser Logs API](https://apis.io/collections/kernel/open-kernel-browser-logs-api/)
- [Kernel API Keys Browser Playwright API](https://apis.io/collections/kernel/open-kernel-browser-playwright-api/)
- [Kernel API Keys Browser Pools API](https://apis.io/collections/kernel/open-kernel-browser-pools-api/)
- [Kernel API Keys Browser Processes API](https://apis.io/collections/kernel/open-kernel-browser-processes-api/)
- [Kernel API Keys Browser Replays API](https://apis.io/collections/kernel/open-kernel-browser-replays-api/)
- [Kernel API Keys Browser Telemetry API](https://apis.io/collections/kernel/open-kernel-browser-telemetry-api/)
- [Kernel API Keys Browsers API](https://apis.io/collections/kernel/open-kernel-browsers-api/)
- [Kernel API Keys Credential Providers API](https://apis.io/collections/kernel/open-kernel-credential-providers-api/)
- [Kernel API Keys Credentials API](https://apis.io/collections/kernel/open-kernel-credentials-api/)
- [Kernel API Keys Deployments API](https://apis.io/collections/kernel/open-kernel-deployments-api/)
- [Kernel API Keys Extensions API](https://apis.io/collections/kernel/open-kernel-extensions-api/)
- [Kernel API Keys Invocations API](https://apis.io/collections/kernel/open-kernel-invocations-api/)
- [Kernel API Keys Managed Auth API](https://apis.io/collections/kernel/open-kernel-managed-auth-api/)
- [Kernel API Keys Organization API](https://apis.io/collections/kernel/open-kernel-organization-api/)
- [Kernel API Keys Profiles API](https://apis.io/collections/kernel/open-kernel-profiles-api/)
- [Kernel API Keys Projects API](https://apis.io/collections/kernel/open-kernel-projects-api/)
- [Kernel API Keys Proxies API](https://apis.io/collections/kernel/open-kernel-proxies-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Kernel Openapi Overlay](https://apis.io/overlays/kernel/kernel-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Kernel Authentication](https://apis.io/security/kernel/kernel-authentication/)
- [Kernel Domain Security](https://apis.io/security/kernel/kernel-domain-security/)
- [Kernel Trust Center](https://apis.io/security/kernel/kernel-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Kernel Scopes](https://apis.io/scopes/kernel/kernel-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kernel.sh)
- [Documentation](https://kernel.sh/docs/)
- [Getting started](https://kernel.sh/docs/introduction/)
- [API reference](https://kernel.sh/docs/api-reference/)
- [Pricing](https://www.kernel.sh/pricing)
- [Sign up](https://dashboard.onkernel.com)
- [Support](https://kernel.sh/docs/info/support)
- [Blog](https://www.kernel.sh/blog)
- [Compliance](https://www.kernel.sh/security)
- [Trust centre](https://trust.kernel.sh)
- [GitHub](https://github.com/kernel)
- [Status](https://status.kernel.sh)

## API Evangelist rating

**Kin Score 50.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 54.5 |
| Contract governance | 18.2 |
| Operational transparency | 42.1 |
| Developer ergonomics | 73.2 |
| Access clarity | 18.4 |

**Agent readiness 39.5** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly |

**Regulatory alignment 31.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kernel/](https://apis.io/providers/kernel/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kernel: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kernel/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
