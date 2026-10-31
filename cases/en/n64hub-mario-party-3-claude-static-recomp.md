# Mario Party 3: Claude-assisted recompilation credits community research and the first port

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 12:51:40 Beijing time on October 31, 2026, The Gaming Emporium (@McGroin83) reports n64hub's three separate Mario Party ports. This entry covers only the 2000 Mario Party 3. Supplementary reading used the complete README at commit 817b57711faf51ee694a132d4d6c3db70ff8ad96, dated October 31 at 08:06:28 Beijing time, before the candidate.

Documentation discloses that almost all repository code, documentation and tests were written by Claude agents under human direction and playtesting, not offered upstream where AI code is rejected. N64Recomp translates MIPS to C with N64ModernRuntime, RT64 and RecompFrontend, reusing mariopartyrd/marioparty3 decompilation symbols and mario-party-engine scheduling. The repository started from the first-game recompilation and explicitly credits Rainchus's first MarioParty3-Recomp for locating audio microcode and identifying overlay loaders to hook. Those community results are not relabeled as AI discoveries.

The README reports menus, six boards and minigames on desktop and browser, window-expanded board cameras, backgrounds and HUD, and display-rate interpolation. Game processes use the shared one-thread-per-process scheduler, running one at a time. Documentation lists Windows/Linux x86-64 and up to four local players' controller assignments; browser pages are built from one's own ROM. Only USA 32MiB big-endian .z64 is supported; game files are absent and repository code is GPL-3.0. Complete compatibility, online multiplayer and independent reproduction are not claimed here. No ROM download, dependency installation, build or playtest occurred. REA is unspecified.

Report candidate snapshot: 119 likes, 2,808 views, 11 reposts. Shared three-game post, not this game's separate engagement.

## Sources

- [The Gaming Emporium reports three independent Mario Party projects, October 31, 2026](https://x.com/i/status/2116392641008951793)
- [Supplementary pinned Mario Party 3 README and prior-work credits, October 31, 2026 at 08:06 Beijing time](https://github.com/n64hub/mario-party-3-recomp/blob/817b57711faf51ee694a132d4d6c3db70ff8ad96/README.md)

[中文](../n64hub-mario-party-3-claude-static-recomp.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
