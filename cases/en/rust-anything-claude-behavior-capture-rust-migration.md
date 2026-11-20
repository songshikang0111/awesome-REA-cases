# rust-anything: capture old answers before Claude Code rebuilds slow paths in Rust

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-20
Stage: Needs verification

At 08:21:03 Beijing time on November 18, 2026, codila (@0xCodila) introduces rust-anything: run an old program on ordinary and edge inputs, record its answers, then have Claude Code migrate pieces into Rust with the old API and behavior checks. This extracts runnable behavior, not original source from closed binaries. The 08:31:36 reply then says file writes are checked but network/database calls are unsupported. That is an early boundary, not necessarily the state of later versions.

A November 18 retelling at 14:14:25 claims Node.js search from 10 ms to 0.5 ms, Python slugify 17x, Ruby shellescape 11.8x, browser WASM 11.5x and zero mismatches in over 30,000 cases. Another at 17:57:32 gives search from 143 ms to 6.9 ms and 38,251 matching samples, listing TypeScript, Python, C, Go, Ruby, Java and Claude Code, Codex, Cursor, Gemini CLI, API preservation and single-setting rollback. These are not one benchmark. Up to 20x, free use, no Rust writing and Discord testing remain promotional statements. The 17:57 post has 43 likes, 1,220 views, 3 reposts and 17 replies in its sealed snapshot; other historical snapshots remain in metadata, not independent measurements.

A new candidate at 10:42:45 on November 20 mentions v2.0.0/v2.1.0 and 17,224 byte-identical Prettier runs. The README and real-world document of erkamyaman/rust-anything were read at pinned commit a3f40af, originally dated November 20 at 07:08:15 Beijing time, before the strict 08:00 window and supplementary only. Documentation explicitly says the tool does not translate automatically: an agent or human writes Rust while the tool supplies recording, bridges, diff and gate. MIT is the project's stated license; nothing was installed or run.

The Prettier 3.6.2 example rebuilds printers from formatter code and input/output behavior, parsing with oxc and falling back to original Prettier for an entire file when a construct is unsupported. The project reports 17,224/17,224 recorded runs byte-identical, of which 15,837 format fully in Rust, with 8.1% fallback. This is not 17,224 pure-Rust cases or a complete all-language replacement. The pinned docs list ten languages; HTML, certain configuration formats, embedded languages and parser boundaries remain uncovered. Unknown options and ignored files can also fall back.

Project benchmark conditions are a ten-core Apple M4, 16 GB, macOS 27.3, Node 24.15.0 and Rust release builds, with two runs and outputs compared before timing. For 2,360 covered JS/TS files with a new CLI process per file, times are 128.6/143.4 seconds versus 6.9/7.2 seconds, roughly 19x. Warmed in-process calls on the same set are 4.2x, not universal 19x. Documentation retains the standalone doc printer being slower across the bridge, configuration fixes, gate inspecting only port.rs while dependency crates need manual checks, and app replay without --build replaying the original command without a fallback rate.

The newer README also describes SMTP and other side-effect recording, not proof of universal network/database equivalence. Recording still executes original code with side effects, requiring isolated copies and test data. This collection statically read project reports, not the complete implementation, and reran no cases, benchmarks or fallbacks. The candidate's GitHub star counts were not checked. Matching covers recorded inputs only, and readable code is not a unique original implementation. REA is unconfirmed and status remains unverified.

November 18 initial-post snapshot: 31 likes, 1,651 views, 3 reposts, 10 replies. Up to 20x is unverified; answer matching covers captured inputs only.
November 18 introduction at 14:14:25: 46 likes, 3,270 views, 9 reposts, 8 replies. Its Node.js search 20x, slugify 17x, shellescape 11.8x and WASM 11.5x concern different hot paths. Slugify produces URL identifiers and shellescape escapes shell arguments. The post also lists PHP/C# previews, recording, diff, bench, gate and rollback. Repository documents have now been read, but raw samples, full per-language coverage, rollback and side-effect equivalence remain untested here. Old promotion is not acceptance of the new version.
November 20 sealed candidate: 0 likes, 18 views, 0 reposts, 0 replies. The post's star counts were not checked and engagement does not validate 17,224 matches.

## Sources

- [codila on rust-anything behavior capture and Claude Code migration, November 18, 2026 at 08:21:03 Beijing time](https://x.com/i/status/2122847517725630555)
- [Supplementary same-author reply: file-write versus network/database limits, November 18 at 08:31:36 Beijing time](https://x.com/i/status/2122850172455796799)
- [Supporting candidate: language coverage, named hot paths and performance retelling, November 18 at 14:14:25 Beijing time](https://x.com/i/status/2122936447003136445)
- [New candidate: 143 ms/6.9 ms search, 38,251 samples and API/rollback retelling, November 18 at 17:57:32 Beijing time](https://x.com/i/status/2122992595710472334)
- [Prettier migration and 17,224 matching runs retelling, November 20, 2026 at 10:42:45 Beijing time](https://x.com/i/status/2123607951864635839)
- [Supplement: README pinned to November 20 at 07:08:15 Beijing time, before the candidate window](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/README.md)
- [Supplement: same-commit real-world document, Prettier fallbacks, benchmarks and known limits](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/docs/real-world.md)

[中文](../rust-anything-claude-behavior-capture-rust-migration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
