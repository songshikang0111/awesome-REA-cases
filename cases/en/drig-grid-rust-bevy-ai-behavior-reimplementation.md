# DRIG: AI-assisted Rust/Bevy reconstruction of Race Driver: GRID behavior

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-28
Stage: In progress

At 16:30:09 Beijing time on November 28, 2026, yibie's list update introduces DRIG: a Rust/Bevy engine reconstruction of Codemasters' 2008 racing game Race Driver: GRID, reading data from the player's own PC installation. The same candidate also introduces Sonic 2006, a separate target.

Supplementary reading covers PipeKnight/drig-race-driver's README at 8b360088b4f250871d8380d564613ef0231e1fc2, committed November 27 at 20:50:23 UTC, before the window. The author explicitly credits AI coding agents with most code and mentions a Claude subscription. The workflow studies grid.exe using Ghidra and other tools, rewrites behavior in Rust, and compares original driving, AI and audio recordings plus individual bit-exact routines. Documentation reports driving, events, damage, career and replays working, but calls the project early and experimental, with possible crashes, physics blow-ups, missing features and visual differences. Some replay audio remains missing. Linux testing is reported only under WSLg, not native Linux hardware.

One-to-one behavior is the goal, not established whole-game byte matching. Backlog completion and fixed headless-scenario pass percentages exclude full graphics, audio and interactive races; some driving scenarios still lack automated checks. This collection read documentation only, without building, running or replaying tests. New versions are described as GPL-3.0-or-later, while older Apache 2.0 releases retain those terms. Original game data must be legally supplied by the player and is not distributed here.

Candidate snapshot: 0 likes, 176 views, 0 reposts, 0 replies. The introduction's 4,005 files do not measure completion.

## Sources

- [yibie introduces DRIG and Sonic 2006, November 28, 2026 at 16:30:09 Beijing time](https://x.com/i/status/2126594483777323455)
- [Pre-window pinned README: AI attribution, trace comparisons, status and platform limits, November 27, 2026 at 20:50:23 UTC](https://github.com/PipeKnight/drig-race-driver/blob/8b360088b4f250871d8380d564613ef0231e1fc2/README.md)

[中文](../drig-grid-rust-bevy-ai-behavior-reimplementation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
