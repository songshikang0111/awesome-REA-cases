# Olaz, a native Zalo client: SwiftUI hosts the official renderer, while Claude credit establishes only a visible patch attribution

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-14
Stage: Related project

At 14:26:40 Beijing time on November 14, 2026, AI Geek News (@aigeeknews) introduces a reverse-engineered Zalo client rewritten in Swift for native macOS use. Zalo is a communications app; the target is accessing messages and calls through a native Mac interface, not finding server vulnerabilities. The candidate identifies no model, REA use or reversing process, and supplementary thread retrieval adds no technical text.

A separate public search located the matching qnguyen3/zalo-swift-re (Olaz) project. Its README and reverse-engineering notes at commit c81437e7614ec77e96a005c72bd00ecd4108074b were read. The README explicitly says it does not reimplement Zalo's protocol. It runs the official app.asar renderer headlessly in WKWebView, supplies the interfaces formerly provided by Electron's preload and main process in Swift, and exposes official-client state through SwiftUI. It describes a 450-member preload bridge table generated from the official script and project-reported QR login, chat, sync and calling states. Group creation is marked unverified against a live account; the feature list is not independent acceptance testing.

The notes identify Zalo PC 26.10.20 and an analysis date of October 25, 2026, combining an early demo-engine plan with later SQLite-host notes. That early design section must not override the newer README architecture. A public commit at 20:51:31 UTC on November 11 (04:51:31 Beijing time on November 12) fixes the WebSocket handshake, explaining that a failing earlier call prevented new messages, and includes a Co-authored-by: Claude Opus 5.5 credit. This establishes that the project publicly attributes part of that patch to Claude, not that AI discovered the initial protocol, all 450 interfaces or the entire client. These supplementary documents and the commit predate the candidate window and are checks, not newly retrieved candidates.

The README says first launch obtains the official runtime from VNG and checks its signature. It still depends on official code, rather than being a standalone Swift protocol implementation. It warns that the project is unofficial and may conflict with terms of service; GPL-3.0 is connected with its libsignal component and does not relicense the official runtime. The candidate's short-link destination was not directly checked; project matching came from separate public discovery. Only documents and commit information were read here. No official installer was downloaded, complete patch reviewed, client built, account used or messaging security validated. REA use is unconfirmed; included as a related project with limited visible evidence of AI participation.

Sealed candidate: 0 likes, 9 views, 0 reposts, 0 replies. A co-author credit does not establish AI work volume, quality or independent execution.

## Sources

- [AI Geek News introduces a native Swift Zalo client, November 14, 2026 at 14:26:40 Beijing time](https://x.com/i/status/2121489975040733330)
- [Supplementary Olaz README: official-renderer host architecture and feature limits, pinned at c81437e](https://github.com/qnguyen3/zalo-swift-re/blob/c81437e7614ec77e96a005c72bd00ecd4108074b/README.md)
- [Supplementary reversing notes: Zalo PC 26.10.20 and host interfaces, internal analysis date October 25, 2026](https://github.com/qnguyen3/zalo-swift-re/blob/c81437e7614ec77e96a005c72bd00ecd4108074b/REVERSE-ENGINEERING-NOTES.md)
- [Pre-window WebSocket fix and Claude co-author credit, November 12, 2026 at 04:51:31 Beijing time](https://github.com/qnguyen3/zalo-swift-re/commit/c81437e7614ec77e96a005c72bd00ecd4108074b)

[中文](../zalo-olaz-swift-official-renderer-interop-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
