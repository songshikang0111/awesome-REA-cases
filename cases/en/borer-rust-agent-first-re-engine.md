# Borer: a Rust reverse-engineering engine for AI agents with emulator comparisons

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-20
Stage: Related project

At 06:21 Beijing time on October 26, 2026, prism (@dear_prism) introduced Borer, a Rust engine written from scratch to give AI agents a reverse-engineering tool surface without Ghidra, IDA or Binary Ninja underneath. It has its own loader, lifters, emulator and decompiler, keeps MCP answers compact, and compares decompiled results against emulation. The author says every component is still being improved, not that correctness has been certified for all architectures.

Supplementary lookup found imjustprism/borer and read its README at fixed commit 2e5b49b5a665f0b1772e4122ac84fd11c570d950, dated October 26 at 11:35:23 UTC, or 19:35 Beijing time, after the strict window. This is later documentation, not proof that every feature existed at 06:21. It describes one Rust binary acting as an MCP server without arguments or a CLI with arguments: load a target, triage it, find functions by strings/symbols, decompile, then follow cross-references and data flow. Listed inputs include PE, ELF, Mach-O, raw code and memory dumps. Filtered/paged lists, delta responses and explicit checking scope aim to reduce context overhead.

The README says decompiled C blocks are run from seeded states and compared against machine code, leaving unmodeled instructions as asm markers. This is a project validation design, not a complete formal proof or a result rerun by this collection. It does not guarantee correct analysis of arbitrary binaries or crash-free handling of hostile inputs. Explicit limits include no 32-bit ARM emulation; refusal of taint/layout/solve/unpack/devirt on arm64; no .NET IL or Swift decompilation; Windows-only live reading without breakpoints or writes; and gotos for unproven control structures.

It is included as a related AI reverse-engineering tool project, not a confirmed REA engine. No installer was executed, MCP configuration changed, dependency installed, target loaded or project test run. Speed, memory use, security and recovery rates were not independently checked. The later documentation uses AGPL-3.0-only while noting versions 0.1.0/0.1.1 were MIT; the current license is not projected onto every historical version.

At 23:59:20 Beijing time on November 20, 2026, prism (@dear_prism) introduces a desktop app and AI chat reading binaries through the same engine tools. Relevant README sections at the pre-candidate dfe542874ac305f51ec91c966df88007c95bea58, committed at 18:38:56 Beijing time, describe a Zed-based workspace with function lists, decompile, listing, graph, hex, xrefs and type editing, with Windows the measured platform. The chat screenshot explicitly uses a scripted demo model making two tool calls before answering; it is not a demonstration of a real remote model's reasoning.

New docs list RISC-V decompilation without check headers and no 32-bit ARM emulation. On x86/x86-64, certify compares final text run as C against machine code on the same inputs. The ntdll example agrees on only 20 of 64 inputs, leaves 44 unchecked and reaches two of three blocks; zero differences is not a full pass. Architectures expand with versions, but the older arm64 analysis-tool limits are not assumed removed. Performance and memory figures are project tests on one machine. No engine, desktop installation or model configuration was run here. This remains early-stage tooling, not a guarantee for arbitrary inputs or safety.

Related tool project, not installed or run; emulator comparisons are a scoped project design, not proof of universal equivalence.
The fixed README postdates the window. Architecture/ARM and live-access limitations are retained without backdating capabilities or licensing.
November 20 candidate: 0 likes, missing view count, 0 reposts, 0 replies. Missing views are not zero; the screenshot uses a scripted demo.

## Sources

- [Window candidate: prism introduces Borer, October 26, 2026 at 06:21 Beijing time](https://x.com/i/status/2114482427477246149)
- [Post-window supplementary README and limits at fixed commit 2e5b49b, October 26, 2026 at 19:35 Beijing time](https://github.com/imjustprism/borer/blob/2e5b49b5a665f0b1772e4122ac84fd11c570d950/README.md)
- [prism introduces desktop app and AI chat, November 20, 2026 at 23:59:20 Beijing time](https://x.com/i/status/2123808420851794353)
- [Supplement: relevant pre-candidate README sections pinned to November 20, 2026 at 18:38:56 Beijing time](https://github.com/imjustprism/borer/blob/dfe542874ac305f51ec91c966df88007c95bea58/README.md)

[中文](../borer-rust-agent-first-re-engine.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
