# Rustify: organizing binary-to-Rust reconstruction with REA evidence, product specifications and slice validation

Category: Applications and clients · REA
Record date: 2026-10-29
Stage: In progress

At 15:46:53 Beijing time on October 29, 2026, Runchao Han (@runchao_han) describes Rustify working through Agent Skills with Claude Code, Codex, Cursor and OpenCode, using REA for reversing. Supplementary reading obtained SebastianElvis/rustify's README at pinned commit 1bbc4ba3506f558f448ffaa4372266f2bb89da96, timestamped 2026-10-29T02:33:34Z, before the original candidate window and used as project context only.

Rather than line-by-line translation of decompiled C into Rust, the workflow asks agents to recover product behavior, UX and architecture from binary and runtime evidence. It maintains recovered/ specifications and evidence, an implementation/ Rust repository, and verification/ comparisons. Eight skills cover preparation, REA probes, product/design/architecture discovery, planning, sliced implementation and validation. A ledger connects requirements, evidence, tests, components, modules and gaps; changed target evidence should invalidate stale results.

The README requires local or cloud agents to access REA, target binaries, resources and a compatible runtime; desktop investigation also needs a GUI session. Full-product parity is a workflow goal and gate, not a promise that every target is complete. It links a rustify-doom example, reportedly reconstructed from a stripped doomgeneric binary and Freedoom data, and lists evaluation directions for base64, BLAKE3, HTTP, dialogs, bzip2, Lua, SQLite, Ninja, Doom and macOS iconutil/textutil. Only the README was read here, not acceptance records for those separate targets; none are declared to have passed and supplementary examples are not counted as independent window candidates.

At 23:37:44 that day, Runchao adds in the current window that porting software is useful for training AI models and that REA can extract execution traces from raw binaries, enabling trace validation to measure fidelity objectively. This is a more concrete validation direction than simply claiming parity, but includes no target, trace, error measure or passing record. It does not establish that Rustify already implements or completes all such tests. The new candidate snapshot is 1 like, 10 views and 0 reposts, without replacing the earlier snapshot.

The public project declares Apache-2.0, with upstream-derived tests retaining their own licenses. Target analysis still requires appropriate rights. This collection did not install skills, configure REA, execute binaries, compile Rust or retest parity. Included as an in-progress public workflow tool requiring target-specific validation.

Earlier candidate snapshot: 0 likes, 16 views, 0 reposts; new reply: 1 like, 10 views, 0 reposts. Repository README is earlier supplementary evidence.
Full-product reconstruction and parity are goals. Trace validation is a newly proposed direction, not independently run here; example/evaluation listings are not passing results.

## Sources

- [Runchao Han describes Rustify cross-agent support and REA dependence, October 29, 2026](https://x.com/i/status/2115711957554851944)
- [Supplementary: pinned Rustify README, October 29 at 02:33:34Z, before the original candidate window](https://github.com/SebastianElvis/rustify/blob/1bbc4ba3506f558f448ffaa4372266f2bb89da96/README.md)
- [Runchao proposes execution traces and fidelity validation, October 29, 2026 at 23:37:44](https://x.com/i/status/2115830452510720014)

[中文](../rustify-rea-binary-to-rust-agent-skills.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
