# zniff: a Rust traffic debugger exposing flow queries, replay and rules to Claude/Cursor through MCP

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Related project

At 21:12:56 Beijing time on November 17, 2026, vicanso (@tree_xie) announces the open-sourcing of zniff. It targets HTTP(S) traffic inspection, protocol debugging and rule changes, exposing these through built-in MCP to Claude and Cursor. This is concrete infrastructure for AI-assisted study of application communication, not a report of a particular service being cracked.

The author says its Rust proxy core and NSH native cross-platform UI package as one binary, with WebAssembly compilation and a web/Docker remote console. Listed protocols include HTTP/1.1, HTTP/2 ALPN negotiation, WebSocket and SSE. Listed decoding covers JSON, GraphQL, schema-less Protobuf/gRPC, MessagePack and inline fields, alongside diffs, waterfalls and sequence diagrams. The post also lists 15 rewrite rules/breakpoints, multilingual code export and MCP flow queries, replay and rule editing. These remain product claims, not a guarantee of decrypting arbitrary encrypted traffic or lossless support for every protocol.

Retrieval confirmed the poster and wording. Repository, license, code, captures and MCP sessions were not reviewed; no proxy, certificates or target dependencies were installed. There are no performance or memory measurements, so the comparison with Electron is not treated as a benchmark. REA is unmentioned; status is related-project.

November 17, 2026 sealed snapshot: 2 likes, 45 views, 1 repost, 1 reply. The 15-rule count is the author's, not an audited inventory.

## Sources

- [vicanso announces zniff and MCP capabilities, November 17, 2026 at 21:12:56 Beijing time](https://x.com/i/status/2122679379734253648)

[中文](../zniff-rust-mcp-http-traffic-research-tool.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
