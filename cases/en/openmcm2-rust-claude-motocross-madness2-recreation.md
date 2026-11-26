# OpenMCM2: Claude-assisted Rust reconstruction of Motocross Madness 2 with replacement assets

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-26
Stage: In progress

At 07:12:26 Beijing time on November 26, 2026, The Gaming Emporium (@TheEmporium83) introduces crspytopgn's OpenMCM2 v0.8.3, a from-scratch Rust reconstruction of Rainbow Studios' 2000 motocross game Motocross Madness 2. It credits Andrew Boudreau's earlier decompilation project and Claude Code-assisted development. Listed features include multiple platforms, rebuilt physics, up to 240 FPS, FSR, track creation/export, gyro controls, replay editing, online leaderboards and drivable scenery vehicles. These are the introducer's feature claims, not tests performed by this collection.

Supplementary reading of the public README pins commit b39aae728be0dd71edf634976706da160c9625fe, dated 07:32:10 that day, after the candidate but within the window. It is supplementary documentation, not another candidate. The README identifies one fan developing with Claude Code and testing ride by ride against the original. It supplies no quantified equivalence tests; original-style handling is not proof of complete physics recovery or stable 240 FPS. It confirms macOS Metal, Windows DX12/Vulkan, Linux Vulkan and WebGPU routes, describes track building, replays and browser/desktop networking, and lists 38 new tracks and replacement art in the Free Pack.

The engine repository contains no original game files. Original graphics require an owned game or a separately obtained free demo; the replacement pack can avoid original assets. Other demo tracks are rebuilt using their routes and scenery but new project-created ground and jumps, not recovered complete original tracks. Asset licensing and local-only/no-upload claims were not audited across all assets or network behavior. Full source, releases and tests were not reviewed. No game was downloaded, dependencies installed, engine run or browser demo played. REA is unmentioned.

Sealed candidate: 3 likes, 149 views, 1 repost, 0 replies. 240 FPS is a relayed upper limit, not measured performance.

## Sources

- [The Gaming Emporium introduces OpenMCM2 v0.8.3, November 26, 2026 at 07:12:26 Beijing time](https://x.com/i/status/2125729354743222498)
- [Supplementary pinned README: Claude's role, platforms, replacement assets and original-game boundaries; November 26, 2026 at 07:32:10 Beijing time commit](https://github.com/crspytopgn/openmcm2/blob/b39aae728be0dd71edf634976706da160c9625fe/README.md)

[中文](../openmcm2-rust-claude-motocross-madness2-recreation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
