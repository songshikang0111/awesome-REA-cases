# Static reconnaissance of an Electron directory: Fengshou reports 20 REA nodes and 26 relations, without runtime assurance

Category: Applications and clients · REA
Record date: 2026-11-14
Stage: Analysis test

At 17:15:48 Beijing time on November 14, 2026, Fengshou (@ai_fengshou) says they inspected an Electron application directory using rea-agents' analyze-javascript-application command with JSON output, without installing Ghidra or logging into an account. Electron packages web interfaces as desktop programs. The purpose is reconnaissance before rebuilding features: understanding connections between the main process, preload script and page entry point. The application is unnamed and is not assigned a commercial-client identity here.

The author reports 20 nodes and 26 relations: main.js creates a window, preload.js is attached through webPreferences, and index.html loads renderer.js. The report also counts zero IPC and zero contextBridge exposures. IPC means inter-process communication; contextBridge is one way Electron exposes interfaces to pages. These zeroes are static-report counts, not proof that dynamic communication, hidden calls or security problems are absent. The author explicitly disclaims assurance that it runs and treats the output as reconnaissance only.

Original retrieval confirms author and wording. The attached image, directory contents, raw JSON output and an answer key were not reviewed, and REA was not run here. MIT and 458,000 stars are promotional statements about the tool, not sample size or accuracy, and are not used as validation. This is kept separate from the existing 846-byte IPC and hidden-network-call fixtures: identical input is not established and the reported output differs. Status remains analysis-test with a static-analysis boundary, not complete application decompilation or an already copied feature.

Sealed candidate: 0 likes, 136 views, 0 reposts, 4 replies. The 20 nodes and 26 relations are the author's reading of tool output, not a rerun by this collection.

## Sources

- [Fengshou's Electron static-structure test report, November 14, 2026 at 17:15:48 Beijing time](https://x.com/i/status/2121532538980311508)

[中文](../fengshou-rea-electron-20-node-static-inspection.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
