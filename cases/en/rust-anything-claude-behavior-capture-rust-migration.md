# rust-anything: capture old answers before Claude Code rebuilds slow paths in Rust

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-18
Stage: Needs verification

At 08:21:03 Beijing time on November 18, 2026, codila (@0xCodila) introduces rust-anything as a way to migrate slow parts of an application to Rust without breaking existing behavior. The post lists Python, JavaScript, TypeScript, Go, Ruby, Java and C projects. It describes running old code, saving outputs for ordinary and edge-case inputs as an answer baseline, then having Claude Code rewrite pieces and compare answers before proceeding. This is a project account of extracting behavior from a runnable implementation and rebuilding it, not recovery of original source from a closed binary.

The poster recommends real user inputs, migrating only hot paths and benchmarking old against new before shipping; whole applications could also be migrated piece by piece. Comparisons cover only captured inputs, not every execution path or side effect. A supplementary same-author reply at 08:31:36 says file writes are checked but network and database calls are not yet supported. The checking mechanism and results were not obtained.

Up to 20× speed, free use and writing no Rust are promotional claims without a named application, hardware, sample size, timing method, build artifacts or bills. Thread references to Discord testing lack a test report and do not establish Discord validation of this tool. Original-post and thread retrieval confirm attribution and the proposed workflow, but the repository, license, code and performance data were not obtained and reviewed. No dependencies were installed, old programs run or migrations executed. REA appears only as a separate suggested article at the end, not evidence of its use in this project. Retained as an unverified AI-assisted behavior-reconstruction tool account.

Sealed candidate: 31 likes, 1,651 views, 3 reposts, 10 replies. Up to 20× is unverified; answer matching covers only captured samples.

## Sources

- [codila on rust-anything behavior capture and Claude Code migration, November 18, 2026 at 08:21:03 Beijing time](https://x.com/i/status/2122847517725630555)
- [Supplementary same-author reply: file-write versus network/database limits, November 18 at 08:31:36 Beijing time](https://x.com/i/status/2122850172455796799)

[中文](../rust-anything-claude-behavior-capture-rust-migration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
