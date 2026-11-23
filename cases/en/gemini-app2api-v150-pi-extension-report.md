# Gemini-app2api: after the pi extension, its author clarifies tool calls and harness boundaries

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-23
Stage: Related project

At 14:41:15 Beijing time on November 19, 2026, 野鴨 (@vildanden_ai) says Gemini-app2api v1.5.0 adds a pi extension for using Hydrogen/Neon directly inside pi without starting a separate gemini-app2api server. The specific goal is connecting Gemini app model access to a coding-agent environment, not recovering model weights or internal inference algorithms.

The post explicitly labels the project reverse-engineered and says it uses Gemini app quota, separate from Antigravity. Available models depend on the plan, including free accounts. Hydrogen/Neon preserve the author's names without identifying official model equivalents. The post claims no Gemini app bans have been reported while warning users to accept the risk. Lack of ban reports is not a safety, authorization or long-term compatibility guarantee. Continued use after losing access to another service is not treated as a tested fact here, and restriction-evasion instructions are not supplied.

Retrieval confirms attribution and wording of the Chinese post. Its 15:08:55 English version repeats the release and is not another result. Repository code, extension implementation, revision-test artifacts, sessions and account-restriction records were not obtained; no account was accessed or extension executed. Retained as a related AI-client interoperability project, not evidence of AI performing protocol research. REA use is unknown.

In the November 23 candidate at 16:56:44, the author further describes reverse engineering a proxy, claiming that the original app filters out tool calls and the project restores them, while the caller supplies the entire harness. The author admits that a weakened backend model is only hearsay and cannot be fixed by this work; this is not restoration of a full-capability model. The supplementary parent is a v1.6.5 announcement dated November 22 at 15:20:59, before this window. It claims pi and OpenClaw integrations, fixes for image-heavy long tasks, and a successful four-hour simulated-human e2e run with over a hundred images. The parent provides background to the new explanation, not an additional candidate or independent test. Raw logs, tool-call formats and permission checks remain absent. Filtering and reduced-capability assertions stay attributed to the author.

November 19, 2026 Chinese candidate snapshot: 7 likes, 327 views, 0 reposts, 0 replies. Engagement from the repeated English announcement is not combined and is not independent validation.
November 23 candidate: 0 likes, 14 views, 0 reposts, 1 reply. Four hours and over a hundred images come from the November 22 parent; test artifacts were not read.

## Sources

- [野鴨 announces the Gemini-app2api v1.5.0 pi extension, November 19, 2026 at 14:41:15 Beijing time](https://x.com/i/status/2123305586922246592)
- [Author clarifies tool calls and harness boundaries, November 23, 2026 at 16:56:44 Beijing time](https://x.com/i/status/2124789231512142291)
- [Supplementary pre-window parent: v1.6.5 and a reported four-hour test, November 22, 2026 at 15:20:59 Beijing time](https://x.com/i/status/2124402750318596107)

[中文](../gemini-app2api-v150-pi-extension-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
