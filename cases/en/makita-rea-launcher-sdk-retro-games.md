# REA Launcher SDK: Fabio Makita extracts retro-racing interoperability into an agent-driven framework

Category: Games and preservation · REA
Record date: 2026-11-03
Stage: In progress

At 09:30 Beijing time on November 3, 2026, Fabio Makita (@AkitaOnRails) announces REA Launcher SDK. After making launchers for Colin McRae games, OutRun, Sega Rally and Screamer, he extracted their shared parts so coding harnesses can make new launchers. His suggestion that it should get users 90% of the way is an expectation, not game coverage or a common acceptance score.

The README was read at akitaonrails/rea-launcher-sdk commit 050d3b3ad4b4840efab744fd65b15d17e60787f3, dated November 3 at 09:54 Beijing time. This is later than the candidate but within the window, and supplementary rather than a separate candidate. It assigns research, reversing and coding to agents such as Claude Code, Codex, opencode and Cursor, while people supply games and decisions. Community fixes are researched first, with human checkpoints for findings, options and actual-game verification. Shared components include a Rust core, Windows helpers/UI, Linux/Wine scripts, AppImage packaging and reusable CI.

The goal is configurable execution of players' own old PC games on modern Windows/Linux, not reconstructing complete games or shipping assets. Project rules keep original game folders read-only, use private runtime copies, pin component URLs with SHA-256 checks and require per-game verification before enabling behavior changes by default. Listed headless, Wine and Rust checks are not executions by this collection. No dependencies, launcher build or game was run here. The documented MIT-or-Apache-2.0 licensing does not extend to games or third-party components.

Candidate snapshot: 25 likes, 1,558 views, 2 reposts. The author's 90% estimate is not a test result; project checks were not run here.

## Sources

- [Fabio Makita announces REA Launcher SDK, November 3, 2026](https://x.com/i/status/2117429251741741227)
- [Supplementary pinned SDK README, commit dated November 3, 2026, 09:54 Beijing time](https://github.com/akitaonrails/rea-launcher-sdk/blob/050d3b3ad4b4840efab744fd65b15d17e60787f3/README.md)

[中文](../makita-rea-launcher-sdk-retro-games.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
