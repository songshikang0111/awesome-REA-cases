# decompdecomp: an independent decomp.wtf continuation where byte matching does not mean a whole game is recovered

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-14
Stage: In progress

At 00:50:08 Beijing time on November 14, 2026, Pixel Cherry Ninja (@PixelCNinja) introduces decompdecomp for Claude, Codex and Cursor to recover byte-matching C/C++ from owned games, calling N64 ready, GBA/PS1/GameCube/DS beta and the tool fully local. Supplementary public-repository research located n-delic/decompdecomp and read its README, pinned to 9e19b4d79f8798df626e6216385ac91b3642535d, committed November 13 at 07:47:52 Beijing time. It predates this candidate window and is supporting background, not a new test in this window.

The document describes compiling agent output with the game's original compiler, counting a function as matched only when bytes are identical, parallel agents working on functions and an autopilot handling easy functions first. Crucially, no whole game has been decompiled: exports combine matched C with assembly for the remainder, so rebuilding is not complete C recovery. N64 is Recommended, many other console/PC targets are Beta and some accept only public community decomps. PS1, PS2 and most N64 targets need WSL2 on Windows; macOS has further compiler limitations. Platform and export claims are project documentation, not execution accepted by this collection.

The README explicitly continues Sam Wolfs's decomp.wtf code, which reached 0.10.6 before archival, while stating independent maintenance, no relationship to its original author and no endorsement. This successor is therefore a separate record; the older Decompwtf record remains and its discontinuation report is not applied to the new project. New code is AGPLv3 with a separate original MIT notice. The project asks users to supply games they are entitled to use and not publish recovered game code. Its privacy language has an important exception: game material stays on the computer except for transmission to the chosen model, so fully local must not imply cloud models never receive game content. No installation, ROM import, build, tests or independent matching-log checks were performed here. REA use is unconfirmed; included as in-progress work.

Candidate snapshot: 16 likes, 1,129 views, 0 reposts, 3 replies. No completed whole game, platform claims and the privacy exception come from project docs, not reruns.

## Sources

- [Pixel Cherry Ninja introduces decompdecomp, November 14, 2026 at 00:50:08 Beijing time](https://x.com/i/status/2121284490500981068)
- [Pre-window supplement: project README pinned to a November 13, 2026 at 07:47:52 Beijing-time commit, read later](https://github.com/n-delic/decompdecomp/blob/9e19b4d79f8798df626e6216385ac91b3642535d/README.md)

[中文](../decompdecomp-local-agent-byte-matching-workbench.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
