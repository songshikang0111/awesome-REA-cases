# REA/Wakaru on DGX ARM64: JavaScript-tool wiring and regression self-tests

Category: Applications and clients · REA
Record date: 2026-11-02
Stage: Analysis test

At 20:41 Beijing time on November 2, 2026, a poster shares an AI work receipt: installing Wakaru 1.14.0 ARM64 on a DGX, expanding REA 6.4.0's x64-only gate to x64/arm64, recompiling, and exporting a Wakaru command in two launchers. A Mac mini DeepSeek forwarding layer expands REA tools from eight to ten, adding analyze_javascript_application and recover_javascript_sources. The changes reportedly exist only as local commit 0306f44, not pushed. The goal is AI-callable JavaScript analysis and recovery on ARM64.

The receipt reports recovery exit 0 for a 131,835-byte React DOM 18 UMD file, yielding one module and a source map in 230ms; Babel parser directory analysis succeeds through rea-javascript-application; a Ghidra regression analyzing system ls succeeds. MCP lists 170 tools including the two JS tools, and forwarding-layer tests pass 2/2. Full tests have one team-report.test.js failure for missing bin/cdx, called pre-existing in the receipt; the earlier state was not independently checked.

The tools apply only to new DeepSeek sessions, while the current session still has eight. REA upgrades or reinstalls overwrite the local changes. The receipt reports about 23MiB added and 9MiB of probes; browser-CDP-dependent analyze_web_bundle was not allowed, and a new-session live test is still a next step. No public patch, output artifacts, source-map quality comparison or raw logs are supplied. Successful exit does not establish original-source recovery or support for all JS packages. Nothing was installed or run and no author machine accessed here.

Candidate snapshot: 1 like, 59 views, 0 reposts. Versions, bytes, 230ms, tool counts and tests come from a posted receipt, not independent retesting.

## Sources

- [DGX ARM64 REA/Wakaru adaptation and self-test receipt, November 2, 2026](https://x.com/i/status/2117235562981523901)

[中文](../dgx-arm64-rea-wakaru-javascript-integration-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
