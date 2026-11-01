# mcp-reverse: one MCP entry for static analysis, external debuggers and multiple AI clients

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-01
Stage: Related project

At 16:46:01 Beijing time on November 1, 2026, @MalwareBibleJP, the author account for マルウエアの教科書, introduces mcp-reverse: a single MCP server combining binary static analysis, external debuggers, technical-document search and multi-AI collaboration for Claude, Codex and Cursor. Its background is switching among tools such as Ghidra, IDA and x64dbg in game/anti-cheat research; the post also describes malware-analysis and mobile-format uses. This is a reversing-workbench project, not a report that a particular game has been fully recovered. REA use is not stated.

The candidate lists built-in PE, ELF, Mach-O, DEX, WASM, ZIP, .NET and minidump parsing, string and crypto-constant checks, and byte signatures. Decompilation is forwarded to connected external MCP backends, with result comparison. Its small x86-64/ARM64 emulator is intended for short instruction sequences or decryption loops, not complete target execution. The post also describes a Frida bridge, task handoff, voting, shared JSON knowledge and MCP sampling to ask the client model for decompilation summaries or structure names. These are feature descriptions, not results from running it here.

The README at pinned 1llu50ry/mcp-reverse revision 2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a was additionally read. The commit is dated October 29 at 21:55:39 Beijing time, before the candidate. It shows a 5.0.1 badge, stdio/HTTP entry points, native parsers, external backends and a multi-client mesh, and asks users to analyze only binaries they own or are authorized to examine. However, tool, backend, skill and test counts differ across sections, and an older technology-stack section says Node 18+ whereas the candidate says 24+. No single count or installation-version guarantee is adopted.

The post says anti-cheat risk levels are fixed tables rather than measurements, file scope uses MCP_FS_ALLOW/MCP_FS_DENY with no default restriction, and HTTP authentication is optionally enabled through MCP_AUTH_TOKEN. These remain attributed safety descriptions, not independently audited code/defaults. Local server execution does not mean offline models, and voting does not establish correctness. No dependencies were installed, tools run, debuggers connected or games/samples tested here.

Candidate snapshot: 6 likes, 698 views, 0 reposts. Reading the README is not a functionality or permission audit.

## Sources

- [MalwareBibleJP describes mcp-reverse features and safety limits, November 1, 2026](https://x.com/i/status/2116814004752613748)
- [Supplementary pinned mcp-reverse README, committed October 29, 2026, before the window](https://github.com/1llu50ry/mcp-reverse/blob/2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a/README.md)

[中文](../mcp-reverse-multi-client-binary-analysis-orchestration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
