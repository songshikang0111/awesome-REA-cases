# Log client adapters: matt observes Instagram with REA and Playwright, then searches public clients

Category: Applications and clients · REA
Record date: 2026-11-10
Stage: In progress

At 09:37:13 Beijing time on October 23, 2026, matt (@matthewsoldit) says log was revamped as a native Codex plugin and Claude connector with Claude Duet support, using REA and Playwright to observe internal APIs, with testing and a push to main planned for the following week. Avoiding automated-activity signals and essentially not burning accounts were the author's inferences, not validated account-safety guarantees. The old post was retrieved this round solely to establish the same author and log project, not to re-adjudicate an old candidate.

A new candidate at 06:19:44 Beijing time on November 10 describes log as a messaging/outreach tool spanning X, Slack, Discord and Instagram, intended to give personal AI context scattered across platforms. In the reported adapter workflow, an MCP request scaffolds a platform and opens it in an AdsPower browser. REA and Playwright observe goal-driven interactions and record steps, then analyze JS bundles for actual internal call names and document them. GitHub API searches seek nearby clients by those names; mention frequency and goal coverage inform selection before vendoring a client and configuring a schema. The author explicitly says they watched AI do this on Instagram. One integration account does not establish complete discovery on all platforms or unrestricted long-term account use.

The reported local message index uses BM25, all-MiniLM-L6-v2, HNSW and reciprocal rank fusion. A sending-stage path separately uses jina-embeddings-v5-omni-small and jina-reranker-v3.5 for relevant context; local LFM2.5-VL-450M describes images/videos, AssemblyAI transcribes voice, and Inworld TTS creates speech that is listened back to. The post names twikit, instagrapi, endcord and gabriel clients, curl_cffi and chat-xdk, with SQLite storage and platform WebSocket messages sent into Claude Code. This architecture list does not establish library compatibility, correct decryption, entirely local data processing or end-to-end privacy. External transcription and speech services cannot be omitted just because indexing is local.

The communication analysis earlier in the post covers 20,073 personal messages and roughly 57 million tokens. Draft checking separately cites 66,116 messages and 130 rules; these are different corpus counts. Rapport is a proposed one-record-per-person relationship-scoring extension explicitly not built yet, not a separate delivered product. Personal communication percentages are not client-recovery accuracy.

Complete new and old posts confirm attribution and project continuity; no messages or accounts were accessed. An exact repository, license, code, adapter traces, input/output pairs and regression tests were not inspected. Free/open source is the author's claim, and completion of the old next-week push-to-main plan is not confirmed. Status remains in progress. No detection-evasion or third-party-account access method is supplied. Observable APIs and publicly available clients do not establish permission to automate calls or process data. No browser, client, model or target was run here.

Originally posted October 23, 2026 at 09:37:13 Beijing time; earlier re-review concerned the 08:00–12:00 window.
The old next-week testing and push to main were plans; avoidance of account bans remains unverified.
November 10 sealed candidate: 0 likes, 130 views, 0 reposts. The 20,073 messages/roughly 57 million tokens and 66,116 messages/130 rules are separate reported statistics, not recalculated here.

## Sources

- [Older candidate: log tool, REA/Playwright and next-week testing plan](https://x.com/i/status/2113444602808250641)
- [New candidate: matt's Instagram adapter workflow, log architecture and unbuilt rapport, November 10, 2026 at 06:19:44 Beijing time](https://x.com/i/status/2119917883535040608)

[中文](../rea-playwright-log-tool-platform-adapters.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
