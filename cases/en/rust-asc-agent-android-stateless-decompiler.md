# rust_ASC: stateless APK and DEX queries for agents

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-06
Stage: Related project

At 09:23:00 Beijing time on November 6, 2026, Dopax (@tensorstaff) recommends rust_ASC in an open-source roundup as a DEX/APK tool for agents and mobile researchers, citing about 125 stars. Supplementary lookup finds the matching MG1937/rust_ASC and reads the README at main's commit 0daddfb832b24bd0e43e76a9365eab4673db0cec, dated October 28 at 15:13:22 Beijing time. This older commit establishes tool identity and interface context, not a release in the candidate window.

Documentation describes a Rust implementation of Python ASC that queries compiled artifacts directly without building a global index or persistent disk cache. It searches string/type/method/field references, locates and decompiles individual classes, lists classes/methods/strings and decodes AndroidManifest, with multi-DEX support. Full-APK pseudocode export reuses radguard. Stdio MCP exposes CLI queries by starting a fresh CLI process per call; extends/impl searches remain CLI-only, so the interfaces are not wholly identical. The purpose is supplying locatable Android-code evidence to agents, not automatically rebuilding arbitrary apps.

The project reports string-reference queries taking 55/67/118/136ms on TelegramX, WhatsApp, Grab and TencentQQ, with single-class decompilation at 79/70/111/118ms, compared with JADX figures from the existing ASC suite. A separate 383MB, 41-DEX QQ full-pseudocode export reportedly takes 2.56 seconds with 32 workers. Different APK sizes and single-class versus full-export workloads must not be conflated. Claimed speedups do not establish complete semantics, recompilable output or universal superiority to JADX. The README states Apache-2.0; the license text was not separately reviewed. Only documentation was read here: no APK downloads, dependencies, target execution or benchmark reproduction. AI authorship of the tool and REA participation are not inferred.

Sealed whole-roundup snapshot: 0 likes, 15 views, 0 reposts. The roundup's 125 stars are neither independently checked nor a correctness measure.

## Sources

- [rust_ASC in Dopax's roundup, November 6, 2026 at 09:23 Beijing time](https://x.com/i/status/2118514451947409450)
- [Supplementary pinned README: October 28, 2026 commit, interfaces and project benchmarks](https://github.com/MG1937/rust_ASC/blob/0daddfb832b24bd0e43e76a9365eab4673db0cec/README.md)

[中文](../rust-asc-agent-android-stateless-decompiler.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
