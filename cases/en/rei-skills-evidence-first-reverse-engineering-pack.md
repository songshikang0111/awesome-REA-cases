# REI Reverse Engineer: from 12 skills to a Rust desktop and dual MCP evidence bridges

Category: Applications and clients · REA
Record date: 2026-11-07
Stage: In progress

At 02:07 Beijing time on November 3, 2026, Batuhan (@AtamanCossack) introduces 12 evidence-first reversing skills in REI Skills, covering binaries, APKs, firmware/IoT, Electron, WASM and protocols within a claimed 895-skill library for 21 AI targets. The older README pinned to 94a5c23e4e39b70994c0b32736978f5704b15c23 distinguishes instructions from a separately installed Python 3.10+ workbench: 14 stdio MCP tools, 124 catalog metadata entries and 11 static external adapters requiring explicit authorization. PATH discovery does not establish versions or licensing, and PE/ELF/WASM parsing is bounded. Live Ghidra/IDA/JADX/Frida sessions and morluto/rea integration were planned at that stage. The linked WASM diff demo was not rerun here; 895 skills do not mean 895 successful investigations.

In the new candidate at 23:29:42 on November 7, the same author introduces REI Reverse Engineer, being built with Rust and Python/MCP around binary identity, byte evidence and reproducibility. Name and maintainer lookup found the public standalone workbench repository. This review reads its README and desktop verification document at 78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95, committed at 23:20:32 Beijing time on November 7, within this window. The verification document dates itself November 2: supplementary earlier project testing, not an experiment occurring this window. The existing ID and sources are retained to extend the same REI workbench rather than add another skill-pack entry.

The new desktop is a licensed MIT/Apache-2.0 source fork of Craft Anything, connecting the original Python workbench and separately pinned morluto/rea through local MCP. Upstream REA is pinned to f72638f6b1f1a41851bf321472569c3265556961. The project reports building and opening an unsigned 0.3 preview on Windows 11 x64, Rust 1.97.0, Python 3.14.7 and Node 24.22.1, discovering 14 plus 234 external routes, totaling 248. Its verification record describes the desktop's native engine dispatching Python identification/SHA-256 and upstream REA byte entropy on the same eight-byte synthetic WASM fixture, returning evidence without executing the target. The servers keep separate evidence stores, not a merged database. Full discovery schemas initially exceeded a budget and timed out; the document uses compact discovery schemas while retaining server-side validation. The older planned-only REA integration description no longer characterizes the new desktop bridge. The two-bridge test does not establish implementation of other live analyzers.

The pinned README reports 352 Rust AI/UI/CLI tests and 65 Python tests, with 64 passing and one optional-tool skip. The earlier desktop document lists 127 desktop/UI tests: a different recorded scope, not an additive count. Twelve skills pass structural checks. Experiential streaming and model listing use loopback integration tests; live paid API calls and user OAuth login were not performed. All 248 routes, decompilation accuracy, device behavior and AI rebuild quality remain individually unverified, with 11 moderate dependency advisories still reported. The Python core performs bounded static analysis, not decompilation or target execution. Evidence bundles exclude original binaries, and integrity hashes do not establish semantic correctness. Hosted models may send prompts and tool results off-device. These are project documentation reports, not independent reproduction by this collection. No dependencies were installed, MCP server started, desktop built or credentials read here.

November 3 older snapshot: 1 like, 11 views, 0 reposts. November 7 candidate: 1 like, 10 views, 0 reposts.
The 124 catalog entries, 14 Python tools, 234 upstream tools and 248 routes describe different scopes, not 248 verified capabilities.
The 352 and 127 tests come from the README and earlier desktop record respectively. Of 65 Python tests, 64 passed and one skipped; all are project-reported.

## Sources

- [Batuhan introduces the REI REA skill pack, November 3, 2026](https://x.com/i/status/2117317644756123796)
- [Supplementary pinned REI Skills README: earlier capabilities and optional workbench, November 3, 2026](https://github.com/rootcastleco/rei-skills/blob/94a5c23e4e39b70994c0b32736978f5704b15c23/README.md)
- [Batuhan introduces the REI Reverse Engineer evidence workbench, November 7, 2026 at 23:29:42 Beijing time](https://x.com/i/status/2119089920086061235)
- [Supplementary pinned workbench README: desktop, dual bridges and verification limits, November 7, 2026 commit](https://github.com/rootcastleco/Rei-Reverse-engineer/blob/78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95/README.md)
- [Supplementary desktop verification: self-dated November 2, pinned at the November 7 commit; testing predates this window](https://github.com/rootcastleco/Rei-Reverse-engineer/blob/78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95/docs/DESKTOP-VERIFICATION.md)

[中文](../rei-skills-evidence-first-reverse-engineering-pack.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
