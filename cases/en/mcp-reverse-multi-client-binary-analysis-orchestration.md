# mcp-reverse, now Decompile: one MCP entry for binary analysis and multiple AI clients

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-25
Stage: Related project

At 16:46:01 Beijing time on November 1, 2026, @MalwareBibleJP, the author account for マルウエアの教科書, introduces mcp-reverse: one MCP server for binary static analysis, external debuggers, technical-document search and multiple AI clients including Claude, Codex and Cursor. It addresses switching among Ghidra, IDA and x64dbg in game/anti-cheat research, also listing malware and mobile formats. This is a reversing workbench, not complete recovery of a game; REA use is not stated.

The older candidate lists native PE, ELF, Mach-O, DEX, WASM, ZIP, .NET and minidump parsing, string/crypto-constant and byte-signature checks, and forwarding decompilation to external MCP backends for comparison. Its small x86-64/ARM64 emulator handles short sequences or decryption loops, not full targets. Frida bridging, handoffs, voting, shared JSON knowledge and MCP sampling for summaries or structure names are feature descriptions, not executions here.

Earlier supplementary research read README revision 2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a, committed October 29 at 21:55:39 Beijing time, before the older candidate. It shows 5.0.1, stdio/HTTP, native parsing, external backends and a multi-client mesh, requiring owned or authorized binaries. Tool, backend, skill and test counts differ across sections; an older Node 18+ stack section conflicts with the candidate's 24+, so no unified installation guarantee is made.

The new November 25 17:38:18 candidate introduces 1llu50ry/Decompile as such a workbench, claiming over 230 tools, 60 backends, 6,000 skills, 170 agents, 160 subagents, 190 plugins and 3,000 prompts, with Node 24+. Concrete examples are pak_parse reading UE4/UE5 pak-footer magic 0x5A6F12E1, index offset/size and SHA1; hash_identify locating hash/crypto constants; and file_identify recognizing binary formats. These counts and behaviors remain the new post's account, without implementation review or recounting. Parsing does not establish decryption of encrypted pak archives or completed reversing.

Supplementary public GitHub API retrieval resolves both the old mcp-reverse path and Decompile to repository ID 1405229384, now named 1llu50ry/Decompile. The original case ID and source URLs are retained, adding the rename instead of a duplicate case. This is current identity information at retrieval, not the original rename date or proof that all features existed when the new post appeared.

Older attributed safety descriptions are retained: fixed, unmeasured anti-cheat risk levels, no default MCP_FS_ALLOW/MCP_FS_DENY restriction, and optional MCP_AUTH_TOKEN HTTP authentication. Code/defaults were not audited, and inheritance of these settings by the current version is not certified. Local servers do not imply offline models, and voting does not prove correctness. No dependencies were installed, tools run, debuggers connected or games/samples tested here.

November 1 candidate snapshot: 6 likes, 698 views, 0 reposts. README review is not a functionality or permission audit.
November 25 sealed candidate: 0 likes, 24 views, 0 reposts, 0 replies. New tool/resource counts were not independently audited.

## Sources

- [MalwareBibleJP describes mcp-reverse features and safety limits, November 1, 2026](https://x.com/i/status/2116814004752613748)
- [Supplementary pinned mcp-reverse README, committed October 29, 2026, before the window](https://github.com/1llu50ry/mcp-reverse/blob/2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a/README.md)
- [Secondary account of Decompile pak/constant analysis and its MCP workbench, November 25, 2026 at 17:38:18 Beijing time](https://x.com/i/status/2125524470882517208)
- [Supplementary public API: current identity/rename mapping of the old repository path, retrieved November 25, 2026; not feature validation](https://api.github.com/repos/1llu50ry/mcp-reverse)
- [Supplementary public API: current Decompile repository ID, retrieved November 25, 2026; not the original rename date](https://api.github.com/repos/1llu50ry/Decompile)

[中文](../mcp-reverse-multi-client-binary-analysis-orchestration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
