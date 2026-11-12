# Lemmings for Windows 95: human-led architecture, REA and agents, and 696 reconstructed functions

Category: Games and preservation · REA
Record date: 2026-11-12
Stage: In progress

At 16:30:18 Beijing time on November 12, 2026, yibie (@yibie) introduces Lemmings for Windows 95, emphasizing human architecture and verification with AI assistance rather than crediting an entire old game to a model. Supplementary reading uses NitrosGits/Lemmings-For-Windows-95's README at ad29aa806811dca6cb3716a4f167ad52f6043ac6, committed November 9 at 17:37:56 Beijing time before the candidate. The target is Visual Sciences' Windows version published by Psygnosis in 1995, reconstructed as source for preservation and modern Windows/Wine use.

The docs identify Ghidra for control flow, types and draft pseudocode, with Hopper and REA for basic blocks, control-flow graphs and global references. Under human direction, Google Antigravity, Claude and Codex CLI analyze x86, translate pseudocode to C/C++, propose Pentium-scheduling and register-allocation hypotheses, and design Python searches. Verification uses original Microsoft Visual C++ 2.2 with /Ox, function-byte comparisons and global-memory-layout checks. A separate portable target uses llvm-mingw/GCC and a minimal custom CRT for 32-bit Windows.

The pinned README reports 696/696 matched functions in one EXE and seven DLLs, spanning UI, files, levels, bitmaps, memory, rendering and lemming physics/skills. It explicitly defines byte-identical as compiled function code, not whole EXE/DLL files. Headers, import tables and some relocated addresses still differ; this is not recovery of every original binary byte. It also reports Windows 11 ARM64 VM and Windows CI builds, while research search/debugging scripts and the gameplay harness remain macOS/Linux-only. None was rerun here.

Users need legally obtained original assets and the matching compiler; the docs say sprites, music, levels and other proprietary assets are not included. Only the README was read statically. Full source, AI sessions, per-function outputs and complete playthroughs were not audited, and no build or original game was run. One hundred percent function matching does not prove every portable behavior or whole-file equality. Work remains in progress with project-reported checks.

Sealed whole post: 3 likes, 275 views, 0 reposts, 1 reply. The 696 functions and builds are pinned project-documentation reports, not independent reproduction.

## Sources

- [yibie's introduction to three AI-assisted game projects, November 12, 2026 at 16:30:18 Beijing time](https://x.com/i/status/2120796315898777815)
- [Supplementary pinned Lemmings README committed November 9, 2026 at 17:37:56 Beijing time, before the candidate; methods, status and limitations](https://github.com/NitrosGits/Lemmings-For-Windows-95/blob/ad29aa806811dca6cb3716a4f167ad52f6043ac6/README.md)

[中文](../lemmings-win95-human-led-ai-reconstruction-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
