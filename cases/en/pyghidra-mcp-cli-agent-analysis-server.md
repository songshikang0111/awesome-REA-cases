# PyGhidra-MCP: agent access to Ghidra through a CLI or shared GUI

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-04
Stage: Related project

At 15:39:34 Beijing time on November 4, 2026, a candidate introduces pyghidra-mcp as a command-line MCP server exposing Ghidra to intelligent agents and LLM tooling. A name lookup found clearbluejar/pyghidra-mcp. Supplementary README reading was compared with commit aeaf4d16b0ce09b6dc5e16bb56d204025d2f6f8e, dated November 2 at 21:59:25 Beijing time. That revision is pre-window tool background, not a new release or experiment in this window.

The project uses PyGhidra and JPype to bridge Ghidra's ProgramAPI/FlatProgramAPI into Python and expose MCP. Its README distinguishes headless analysis from --gui sharing live project state, recommends streamable HTTP, requires a running HTTP server for its CLI client, and reserves stdio for MCP hosts unable to connect over HTTP. Documented operations include decompilation, cross-references, bytes, call graphs, symbol/string/code searches, and edits to names, types, prototypes and comments. ChromaDB supplies semantic search and analysis starts asynchronously.

The documentation explicitly calls it an actively developed beta. Included as concrete AI-reversing infrastructure, not a guarantee of decompilation accuracy, successful parallel analysis of arbitrary projects or full semantic recovery. The README mentions unit and integration tests, but CI execution records were not inspected and no server was run, dependencies installed or binaries analyzed here. No relationship to morluto/rea is assumed.

Candidate snapshot: 0 likes, 15 views, 0 reposts. Documented features are not execution results from this collection.

## Sources

- [Candidate introduction to the pyghidra-mcp server, November 4, 2026](https://x.com/i/status/2117884444992512437)
- [Supplementary project README at a November 2, 2026 pinned commit, before this window](https://github.com/clearbluejar/pyghidra-mcp/blob/aeaf4d16b0ce09b6dc5e16bb56d204025d2f6f8e/README.md)

[中文](../pyghidra-mcp-cli-agent-analysis-server.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
