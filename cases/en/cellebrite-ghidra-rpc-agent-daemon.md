# ghidra-rpc: Cellebrite Labs gives agents a persistent Ghidra project through a JSON CLI

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-05
Stage: Related project

Candidates at 09:21:37 and 09:25:15 Beijing time on November 5, 2026 introduce Cellebrite Labs' ghidra-rpc; a Japanese account at 11:04:02 details version 0.3.0. Supplementary research reads the public README pinned to fa3866243dcfcbc876baa7b13ae0deac2c443cd8, committed at 01:02:27 Beijing time on November 3, and the v0.3.0 release published at 01:10:50 that day. These project records predate the candidates and are not new tests in this window.

PyGhidra keeps Ghidra running in a JVM, with a structured-JSON CLI allowing Claude Code, Cursor and similar agents to decompile, trace call graphs and cross-references, rename and annotate, recover types, patch instructions/bytes, match functions with BSim and compare versions. Binaries load once; the documentation says changes are saved after each command and visible in the GUI. Intended uses include binary audits, vulnerability research and patch comparisons. Tool capabilities do not establish a correctly reversed target.

Version 0.3.0 documents token-authenticated TCP on 127.0.0.1 instead of Unix sockets on Windows, headless and GUI support, and a detach fix for launchers using Job Objects. search-decompiled reports actual coverage and the next unscanned address for bounded resumption; xrefs-to follows import thunk chains. Consistently 0x-prefixed output addresses, treating bare hex as names, and omitting the instructions array from default disassemble output are compatibility changes. The release also reports fixing aborted write transactions that could discard the next successful write when saving, and retaining old types if --or-replace fails.

The project reports unit CI on three operating systems and Windows headless integration, but no GUI CI. GUI mode rejects version-track and match-function. README prerequisites are Ghidra 11+, Python 3.11+, Java 17+ and uv, with an MIT license. This review checked documentation and release records, not all implementation, CI execution, dependencies or binaries. Release fixes are not independent reproduction, proof of semantic correctness or blanket platform guarantees. Use of morluto/rea is unconfirmed.

Sealed candidates respectively: 0 likes/22 views/0 reposts; 0/43/0; 1/431/3. The roundup's 394 stars is only a relayed November 5 snapshot.
Test coverage and fixes are project reports; GUI is outside CI and nothing was run here.

## Sources

- [Candidate: open-source roundup mentions ghidra-rpc, November 5, 2026 at 09:21:37](https://x.com/i/status/2118151716223017172)
- [Supporting candidate: daemon, JSON and agent uses, November 5, 2026 at 09:25:15](https://x.com/i/status/2118152633903132784)
- [Supporting candidate: Japanese account of v0.3.0 and GUI limits, November 5, 2026 at 11:04:02](https://x.com/i/status/2118177490820898823)
- [Supplementary project README pinned to a November 3 commit, not this window's test](https://github.com/cellebrite-labs/ghidra-rpc/blob/fa3866243dcfcbc876baa7b13ae0deac2c443cd8/README.md)
- [Supplementary project release: v0.3.0, November 3, 2026 at 01:10:50 Beijing time](https://github.com/cellebrite-labs/ghidra-rpc/releases/tag/v0.3.0)

[中文](../cellebrite-ghidra-rpc-agent-daemon.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
