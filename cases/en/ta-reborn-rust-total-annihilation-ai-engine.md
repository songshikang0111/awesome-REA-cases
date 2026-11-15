# TA Reborn: a Claude-assisted Rust Total Annihilation engine using owned game data, not recompiling the original EXE

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-15
Stage: In progress

At 16:30:12 Beijing time on November 15, 2026, yibie (@yibie) describes TA Reborn as a new Rust engine rewritten from scratch and points to Claude Opus development credits. Its target is a modern engine reading units, maps and campaigns from a legitimately owned copy of 1997's Total Annihilation, not original-source recovery or EXE recompilation. It is a different repository and implementation from the baseline Go project Nanolathe, so the shared original game does not justify merging them.

Supplementary research read the README at Jared-woodruff/TA-Reborn commit 49186900c846f875c628eada350fc07b8d5dc62e, committed November 15, 2026 at 11:39:28 UTC, after the candidate but still inside the window. It is corroboration, not an additional candidate. The document names Jared Woodruff as project lead, Claude Opus 5.5 as DEV and GPT6 Astra as QA, while thanking decades of community file-format research. Clean-room is the project's characterization, not an audit here. It describes HPI/GAF/3DO/COB formats, a COB script VM, a 30 Hz fixed-point simulation, wgpu rendering and its own lockstep multiplayer.

The same page advertises 20,000 units, campaigns, mods, replays and multiplatform packages. This collection measured no frame rates, completed no campaigns and checked no compatibility. Documentation explicitly rules out multiplayer with original-game clients and says tests requiring game data skip when no installation is found. Passing basic tests therefore cannot establish complete equivalence. The README presents the current development build while linking release 1.0.6; not every development feature is promoted to verified release functionality.

The candidate's 2,071 files were not independently counted and are not a measure of labor. The project requires owned game data and supplies no original units, maps, art or audio. It states GPLv3-or-later for its engine, with separate music rights; open source does not make the original game free. This collection downloaded no game or release, built or ran nothing and did not inspect all commits to quantify AI contribution. REA is unmentioned; retained as in progress with project-report limits.

Whole candidate post: 8 likes, 533 views, 0 reposts, 7 replies. 2,071 files is the commentator's uncounted figure.
20,000 units, 30 Hz and 1.0.6 are project-documentation figures, not performance tests here. AI credits do not quantify contribution shares.

## Sources

- [yibie introduces TA Reborn's Rust engine and Claude attribution, November 15, 2026 at 16:30:12 Beijing time](https://x.com/i/status/2121883453767688434)
- [Post-candidate pinned README corroboration: architecture, credits and limits, committed November 15, 2026 at 11:39:28 UTC](https://github.com/Jared-woodruff/TA-Reborn/blob/49186900c846f875c628eada350fc07b8d5dc62e/README.md)

[中文](../ta-reborn-rust-total-annihilation-ai-engine.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
