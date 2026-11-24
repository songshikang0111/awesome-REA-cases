# browser-capture: CY describes CDP traffic and call-stack collection for agents

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-25
Stage: Related project

At 02:00:02 Beijing time on November 25, 2026, CY (@AIchanyi) introduces browser-capture as a way to turn authorized web research from single-request inspection into a traceable evidence chain. It reportedly uses Chrome DevTools Protocol with BitBrowser, AdsPower or Chrome/Chromium/Brave/VisibleV8 in stealth, standard and deep modes. The post claims Node.js 22, no third-party dependencies, a CLI and SKILL.md for Claude Code/Codex. It describes SHA-256 deduplication of static and eval code from pages, iframes and workers; Wasm binaries/export tables; HTTP, WebSocket, SSE and NDJSON traffic; DOM storage and crypto.subtle information, with response bodies up to 16 MiB.

It also claims no Runtime.enable by default, concealed hooks, debugger replacement preserving positions/length, local overrides, correlation through up to 32 asynchronous stack-parent levels and HAR 1.2 export. These are the introducer's claims, not source-reviewed or anti-detection-tested features. Repository, revision, skill text and a named capture sample were not obtained through the short link. No implementation relationship to XCrun's earlier web skill is established, so its authorship is not borrowed.

Claimed loopback-only CDP/browser-API connections to 127.0.0.1 or localhost establish neither no external browser traffic, no disk capture nor no leakage risk. Listed cookies, storage and responses can contain sensitive material. No browser, account traffic, dependency installation or code execution was involved here. Retained as a related research tool, not recovery of server implementations from captured client code. REA is unmentioned.

Sealed candidate: 1 like, 34 views, 0 reposts, 0 replies. Features, limits and dependencies are secondary claims without implementation or capture checks.

## Sources

- [CY's complete browser-capture and agent-skill introduction, November 25, 2026 at 02:00:02 Beijing time](https://x.com/i/status/2125288347731906893)

[中文](../browser-capture-cdp-agent-reverse-engineering-tool.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
