# Mario Party 2: n64hub's Claude-assisted native and browser recompilation

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 12:51:40 Beijing time on October 31, 2026, The Gaming Emporium (@McGroin83) reports n64hub's three independent Mario Party static-recompilation projects. This entry is the 1999 Mario Party 2, not an extra mode in the first port. Supplementary reading used the complete README at commit bd4ee2d474d6ca4cffe178669549300880b59659, dated October 31 at 08:07:23 Beijing time, before the candidate.

The README says almost all repository code, documentation and tests were written by Claude agents under human direction and playtesting, with no contributions offered to upstream projects that reject AI code. N64Recomp translates game MIPS into C, while N64ModernRuntime, RT64 and RecompFrontend provide native execution and presentation. It reuses mariopartyrd/marioparty2 decompilation symbols and the shared mario-party-engine process scheduler. Existing community work is not credited as independently accomplished by this author or AI.

Documentation reports menus, six boards and minigames running on desktop and browser, with board views, backgrounds and player panels fitted to the window and interpolated to its refresh rate. The shared scheduler runs each game process on its own thread, one at a time. Browser pages are built from one's own ROM; Windows/Linux x86-64 release paths and up to four local players' controller assignments are documented. Only the USA 32MiB big-endian .z64 is supported. No ROM or game assets are included; repository code is GPL-3.0. No game or release download, dependency installation, build or playtest occurred here. README status is not complete-compatibility acceptance. REA is unspecified.

Report candidate snapshot: 119 likes, 2,808 views, 11 reposts. Shared three-game post, not this game's separate engagement.

## Sources

- [The Gaming Emporium reports three separate ports, October 31, 2026](https://x.com/i/status/2116392641008951793)
- [Supplementary pinned Mario Party 2 README, October 31, 2026 at 08:07 Beijing time](https://github.com/n64hub/mario-party-2-recomp/blob/bd4ee2d474d6ca4cffe178669549300880b59659/README.md)

[中文](../n64hub-mario-party-2-claude-static-recomp.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
