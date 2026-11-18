# rust-anything: capture old answers before Claude Code rebuilds slow paths in Rust

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-18
Stage: Needs verification

At 08:21:03 Beijing time on November 18, 2026, codila (@0xCodila) introduces rust-anything to migrate slow application paths to Rust without breaking behavior. The post lists Python, JavaScript, TypeScript, Go, Ruby, Java and C, describing running old code, recording ordinary/edge-case outputs as an answer baseline and having Claude Code rewrite pieces with comparisons. This extracts and reconstructs runnable behavior, not original source from a closed binary. The author recommends real inputs, hot-path-only migration and speed comparisons before delivery, or whole-app migration piece by piece. A same-author reply at 08:31:36 says file writes are checked but network/database calls are unsupported; the checking mechanism and results were not obtained.

The early up-to-20x, free-use, no-Rust-writing and Discord-testing statements are promotional and lack original experiments; they do not establish Discord validation. A 14:14:25 retelling gives Node.js search from 10 ms to 0.5 ms, Python slugify 17x, Ruby shellescape 11.8x, browser WASM 11.5x and zero mismatches in over 30,000 cases, with PHP/C# in preview. Detailed numbers and historical engagement remain in metadata. Different hot paths do not establish universal whole-app speedups.

A new candidate at 17:57:32 says the creator's demo runs the same search in 143 ms in TypeScript versus 6.9 ms in Rust, replaying 38,251 recorded cases with zero mismatches. It lists six languages—TypeScript, Python, C, Go, Ruby and Java—plus Claude Code, Codex, Cursor and Gemini CLI, preserving the old API, selecting pieces and switching a piece back with one setting. The post contains two promotional versions, not two independent experiments. The 143/6.9 and earlier 10/0.5 figures are different retellings, not a single benchmark or grounds for a universal speed ratio. The new sealed candidate has 43 likes, 1,220 views, 3 reposts and 17 replies on November 18, not implementation acceptance.

The original post and early thread confirm attribution and workflow; the new post remains a secondary demo account. Repository, license, code, raw samples, hardware, timing/build setup, bills and rollback tests were not obtained and reviewed. Zero mismatches constrains recorded inputs only, not every path or side-effect equivalence, nor resolution of the earlier network/database limits. No dependencies were installed, old programs run or migrations executed. REA is a separate suggested reading topic, not evidence of use in this project. Status remains unverified.

Sealed candidate: 31 likes, 1,651 views, 3 reposts, 10 replies. Up to 20× is unverified; answer matching covers only captured samples.
A later introduction at 14:14:25 Beijing time on November 18 claims Node.js search improves from 10 ms to 0.5 ms, or 20×; Python slugify 17×; Ruby shellescape 11.8×; browser WASM 11.5×; and zero mismatches across over 30,000 cases. It lists Node.js/TS, Python, C, Go, Ruby and Java, with PHP/C# in preview, and describes recording, diff, bench, gate and rollback. Slugify converts strings to URL identifiers; shellescape escapes shell arguments. These are different hot paths, not universal application speedups. No repository, raw samples, hardware, timing/build setup, per-language coverage or rollback tests were obtained. Zero mismatches constrains only the samples used, not network/database side-effect equivalence or resolution of the earlier unsupported paths. Sealed candidate: 46 likes, 3,270 views, 9 reposts, 8 replies. Nothing was installed or run here.

## Sources

- [codila on rust-anything behavior capture and Claude Code migration, November 18, 2026 at 08:21:03 Beijing time](https://x.com/i/status/2122847517725630555)
- [Supplementary same-author reply: file-write versus network/database limits, November 18 at 08:31:36 Beijing time](https://x.com/i/status/2122850172455796799)
- [Supporting candidate: language coverage, named hot paths and performance retelling, November 18 at 14:14:25 Beijing time](https://x.com/i/status/2122936447003136445)
- [New candidate: 143 ms/6.9 ms search, 38,251 samples and API/rollback retelling, November 18 at 17:57:32 Beijing time](https://x.com/i/status/2122992595710472334)

[中文](../rust-anything-claude-behavior-capture-rust-migration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
