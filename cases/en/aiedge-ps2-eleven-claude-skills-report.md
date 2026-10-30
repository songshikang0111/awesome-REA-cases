# The Console skill: eleven Claude skills organize PS2 recompilation and mod work

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-30
Stage: In progress

At 13:00:03 Beijing time on October 30, 2026, AI Edge (@aiedge_) describes eleven Claude Code skills for PS2 reversing, graphics, sound, controllers and code mods. Supplementary public search found the closely corresponding Jakeschincariol/console-skill. Its README was read at a508929f1e8f5dd6f54afe489fd74340df3b6f74, committed October 22 at 22:14:44 Beijing time, before the window, with Claude Opus 5.5 co-authorship. The candidate short link was not resolved; this repository corroborates the matching description, not a confirmed short-link destination.

Documentation describes native porting built on ran-j/PS2Recomp and hkmodd's original skill, not an emulator: MIPS machine code is recompiled to C++, while agents fill in runtime functionality and examine Ghidra functions and crash logs. Shared STATE.md and design.md retain stages and behavior specifications. The eleven roles also cover levels, physics, saves, multiplatform packaging and testing. Widescreen, arbitrary controllers, mods and cloud sync are documented claims, not individually accepted functionality here.

The project claims 559 offline tests on synthetic ELFs, discs, textures, audio, memory cards and logs without real game data; that does not mean 559 games pass. The README says many games do not boot, graphics and vector-unit code are slow, many stubs remain and porting may take weeks or fail. Users must supply legally obtained games, and generated C++ and assets should not accompany published patches. The toolkit's MIT license and PS2Recomp's GPL-3.0 do not license all targets. No games were downloaded, skills installed, ports compiled or tests rerun here. One-click playability and universal platform support are not established.

Candidate snapshot: 3 likes, 1,842 views, 1 repost. The project's 559 synthetic tests were not independently run.
Pinned commit: 2026-10-22T14:14:44Z. Candidate short-link destination unconfirmed.

## Sources

- [AI Edge introduces eleven PS2 Claude skills, October 30, 2026](https://x.com/i/status/2116032360559108398)
- [Supplementary: closely matching console-skill pinned README, October 22 commit](https://github.com/Jakeschincariol/console-skill/blob/a508929f1e8f5dd6f54afe489fd74340df3b6f74/README.md)
- [Supplementary: pinned commit and Claude co-authorship](https://github.com/Jakeschincariol/console-skill/commit/a508929f1e8f5dd6f54afe489fd74340df3b6f74)

[中文](../aiedge-ps2-eleven-claude-skills-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
