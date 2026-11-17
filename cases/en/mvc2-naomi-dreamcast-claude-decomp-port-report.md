# Marvel vs. Capcom 2: Claude-assisted decompilation, with public docs separating code matches, ROM reuse and ports

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-17
Stage: Needs verification

At 01:02:06 Beijing time on November 16, 2026, Pixel Cherry Ninja (@PixelCNinja) relays Claude-assisted decompilation of Marvel vs. Capcom 2's NAOMI arcade and Dreamcast releases and PC/3DS ports. At 11:59:43 on November 17, The Gaming Emporium (@McGroin83) adds developer gibletto, a v0.4 arcade test menu, Windows GPU rendering, CHD/GDI/CUE/BIN/ISO disc inputs and a 60 fps claim for every 3DS/2DS model. Both are project introductions, not independent reproductions.

Supplementary research located gibletto/mvc2-naomi-dc and read README and ports/README at 4ccf4b47496c015e4c629403b682905d9838800a. This pre-window commit, November 16 at 20:41:11 Beijing time, describes adding the test menu and fixing 3DS tile gaps. README explicitly discloses Claude and says one C/SH-4 assembly tree matches export and US arcade programs, the Dreamcast main program and 354 character overlay files. It supplies program sizes and SHA-1 targets and reports 18,306 arcade routines in 700 files and 18,991 Dreamcast routines in 773 files. Only documentation was read: no comparisons were run or target hashes recomputed, and uniquely recovered original source is not established.

Important limits: matching builds require specific Hitachi SHC 5.1 Release 08 tools and Sega SDK libraries. Of 301 library modules, 260 reuse SDK objects directly and 41 are reportedly decompiled. The arcade build also extracts seven unused models, 16 KB of older-build residue and an 8 KB Z80 program from the user's ROM. Whole-ROM identity therefore does not mean every byte comes from recovered source. README acknowledges unnatural or nonexecuting statements in some routines to obtain matches.

Port documentation says game code compiles for the host, but missing library routines have stubs, AICA sound still emulates ARM7 and DSP, and the 3DS disables DSP with optional simplified reverb. Not being a traditional emulator does not mean no emulation. Windows uses SDL_GPU with Direct3D 12 or Vulkan and software fallback. The documented 59.94 fps game cadence is not performance measured here. 32-bit ARM Linux is described as buildable but not yet run; x86 Linux still lacks support pieces. 3DS memory and CIA/3dsx differences preclude treating publicity as full all-model equivalence.

Users need original game assets. Project code is labeled AGPLv3; this does not authorize original material or SDK redistribution. A v0.4-tag API query returned 404 and the actual release tag was not confirmed; that is not evidence the project does not exist. No target games, SDKs, build artifacts or dependencies were downloaded; no videos, games, complete source/CI or test matrix were reviewed or run. REA is unmentioned. Status remains other-ai/unverified: public docs strengthen evidence, not establish reproduction.

November 16 sealed snapshot: 88 likes, 2,391 views, 11 reposts, 7 replies; retained unchanged.
November 17 sealed candidate: 1 like, 51 views, 0 reposts, 0 replies. Both 100% and 60 fps remain project/secondary claims, not independent tests.

## Sources

- [Pixel Cherry Ninja on MVC2 decompilation, Claude and ports, November 16, 2026 at 01:02:06 Beijing time](https://x.com/i/status/2122012277172052221)
- [The Gaming Emporium on gibletto, v0.4 and PC/3DS features, November 17 at 11:59:43 Beijing time](https://x.com/i/status/2122540157496602800)
- [Pre-window supplement: pinned README on Claude disclosure, matching scope and ROM reuse, November 16 commit](https://github.com/gibletto/mvc2-naomi-dc/blob/4ccf4b47496c015e4c629403b682905d9838800a/README.md)
- [Pre-window supplement: pinned port docs on rendering, stubs, audio and platform limits](https://github.com/gibletto/mvc2-naomi-dc/blob/4ccf4b47496c015e4c629403b682905d9838800a/ports/README.md)

[中文](../mvc2-naomi-dreamcast-claude-decomp-port-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
