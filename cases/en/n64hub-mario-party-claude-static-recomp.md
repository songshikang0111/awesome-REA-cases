# Mario Party: n64hub uses Claude-assisted static recompilation for desktop and browser

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 12:51:40 Beijing time on October 31, 2026, The Gaming Emporium (@McGroin83) reports n64hub's Mario Party trilogy, explicitly three separate projects. This entry covers only the 1998 first game. Supplementary reading used the complete README at commit ac7f9b52fc07ecbf20b180ef4854563e2d0c610b, dated October 31 at 08:06:58 Beijing time, before the candidate. The other games have separate entries.

The project translates original N64 MIPS code to C through N64Recomp and runs it natively with N64ModernRuntime, RT64 and RecompFrontend. It reuses symbols from the community mariopartyrd/marioparty decompilation, not an entirely new Claude recovery of all game code. The README says almost all code, documentation and tests in this repository were written by Claude agents, directed and play-tested by a person, and are not offered to upstream projects that reject AI-written code. A shared mario-party-engine scheduler handles the game's setjmp/longjmp process switching with one thread per process, running one at a time, on both desktop and browser.

The project reports working boards and minigames, RT64-expanded views, backgrounds and HUD, display-rate interpolation, and browser pages built from one's own ROM. Documentation lists Windows and Linux x86-64 release paths and controller assignment for up to four local players. Only the USA 32MiB big-endian .z64 is supported; no ROM or game assets are included. No ROM, dependencies or release package was downloaded, and no build, playtest, browser or compatibility verification occurred here. Playability and platform coverage remain project reports, not proof that every minigame passes. This repository uses GPL-3.0; the original game and upstream work retain their rights.

Report candidate snapshot: 119 likes, 2,808 views, 11 reposts. The post covers all three games; these are not separate per-game engagement figures.

## Sources

- [The Gaming Emporium reports three independent Mario Party ports, October 31, 2026](https://x.com/i/status/2116392641008951793)
- [Supplementary pinned first-game README, October 31, 2026 at 08:06 Beijing time](https://github.com/n64hub/mario-party-recomp/blob/ac7f9b52fc07ecbf20b180ef4854563e2d0c610b/README.md)

[中文](../n64hub-mario-party-claude-static-recomp.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
