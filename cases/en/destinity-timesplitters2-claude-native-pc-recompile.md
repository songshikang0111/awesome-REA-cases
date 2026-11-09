# TimeSplitters 2: Destinity and Claude recompile the PS2 game, tracing differences against PCSX2

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-10
Stage: In progress

At 01:43:29 Beijing time on November 10, 2026, Destinity (@blackintrax) describes building a native-PC TimeSplitters 2 with Claude: the maintainer play-tests and decides, AI does much of the reversing, every fix is checked frame by frame against PCSX2 and the tooling is GPL-3.0. Supplementary posts at 01:43:24 and 01:43:28 report PS2-to-x86 recompilation, 60 FPS, true 16:9 and up to 4K, with Linux/Steam Deck playable and Windows/online pending. A launcher builds locally from the user's own disc image; about three minutes is the author's estimate.

Supplementary reading covers README, VERIFICATION and KNOWN_ISSUES in Destinity13/TimeSplitters-2-Native-Linux-Recomp at 55722bd4e41937a6dac8c81dcd2fea821412caee, committed November 9 at 18:06:01 Beijing time, before this window. A PS2Recomp fork translates R5900 MIPS to C++ and VU1 to C++/SSE before native compilation. There is no runtime CPU emulation, but PCSX2 GS and SPU2 still supply graphics and sound; parts of the kernel, I/O and timing are implemented at a high level by the runtime. Native does not mean independent of emulator components. The docs credit Claude with reversing, implementation, measurement and documentation, while a human controls direction, hardware and play-testing.

Verification describes input replays, screenshots, savestate registers, RAM and logs to locate the first difference, claiming matching registers and GS output across 10.9 million VU1 calls on a reference route. It explicitly says the in-house test/reference tooling is unpublished, so the full checks cannot be replayed from this material. The known-issues document separately retains a differing end-of-program CLIP register at 0x18d8 due to roughly 90 cycles of timing difference, reportedly without a visible effect. Route-specific results are not universal identity of every state bit.

The project reports completing Siberia on PC/Deck, including two-player co-op, and working Arcade League, Challenge and MapMaker. Story levels 2–10, Arcade Custom and three/four-player play remain untested. Some character-preview menus run at 49–56 FPS versus about 59.9 FPS in main menus/gameplay, and audio fixes are still being play-checked. Windows and online for up to 16 players are described as built but pending release 1.0, with internet play still needing tests: neither general availability nor a whole-game playthrough is established. Users need their own USA SLUS-203.14 disc; source licensing does not authorize the game. No game was downloaded, build or test tooling run, or play-test performed here. These are public project records, not independent reproduction. REA is unmentioned.

Sealed candidate: 0 likes, 11 views, 0 reposts. Supplementary thread posts identify the project without replacing the candidate.
Pinned commit: 2026-11-09T10:06:01Z. The 60 FPS, 4K, 10.9 million calls and three-minute figures are project claims, not independently rerun.

## Sources

- [Candidate: Destinity discloses Claude reversing, human play-testing and PCSX2 comparison, November 10, 2026](https://x.com/i/status/2119848363772248275)
- [Supplementary thread: native-PC TimeSplitters 2 and platform stages, November 10, 2026 at 01:43:24 Beijing time](https://x.com/i/status/2119848340917797362)
- [Supplementary thread: local builds from an owned disc, November 10, 2026 at 01:43:28 Beijing time](https://x.com/i/status/2119848361423520203)
- [Pre-window pinned README: architecture, status and AI disclosure, November 9, 2026 commit](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/README.md)
- [Verification at the same commit: unpublished internal tools and VU1 route comparison](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/docs/VERIFICATION.md)
- [Known issues at the same commit: November 8 v0.9.9 record and untested scope](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/docs/KNOWN_ISSUES.md)

[中文](../destinity-timesplitters2-claude-native-pc-recompile.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
