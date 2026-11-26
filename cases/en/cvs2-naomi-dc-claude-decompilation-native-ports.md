# Capcom vs. SNK 2: Claude-assisted three-version decompilation, separating byte matching from native ports

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-26
Stage: Needs verification

The candidate at 16:01:36 Beijing time on November 26, 2026 introduces gibletto's Capcom vs. SNK 2 v0.0.1. It claims 100% byte matching for the 2001 fighting game's Japanese and US NAOMI arcade releases and Japanese Dreamcast program, plus Windows, Linux, 3DS, PSP and MiSTer ports. It follows Marvel vs. Capcom 2's tools and structure but targets a different game, and is not the collected Capcom vs SNK-to-SNES plan.

Supplementary reading covers the root README and ports/README at e3408908e9e9af696bada01e7281a5ac296282ef, committed November 26 at 16:49:05 Beijing time. These are documents after the candidate, not another candidate or tests run by this collection. The root explicitly discloses Claude use and now identifies release 0.0.2. The project rewrites all three versions' machine code as C, retaining SH-4 assembly where the original was assembly, with conditional builds from one source tree. Retained symbols in the US PS2 program supply about 9,700 routine names; structures, fields and other names are reconstructed or assigned. The docs report about 11,300 Japanese arcade routines, including about 9,800 Capcom routines in 285 files, and about 15,600 Dreamcast routines, with game code in 358 files. Byte identity does not prove uniquely recovered original source; the docs acknowledge some unnatural matching constructs.

Build documentation lists expected program/image SHA-1 values and checking steps, not hashes produced by execution here. The large arcade image reuses art, sound and other data plus 8 KB of Z80 code from an owned disc. The Japanese arcade game links 300 SDK modules unchanged and builds 19 more; Dreamcast links 467 and builds another 39. A matching image does not mean AI recovered every asset, library or auxiliary-processor program. Matching original programs also requires specific Hitachi tools and Sega SDKs. Users must obtain the required material lawfully; this collection distributes none of it.

Port documentation says it compiles the game's C and implements host layers, while audio still uses the original driver with ARM7/DSP emulation or a C implementation. Original-program matching does not automatically establish equivalent behavior or rendering on new hosts. PC uses SDL GPU with Direct3D 12/Vulkan; Linux is 32-bit x86; PSP supports only Dreamcast. Dreamcast networking cannot reach the original server, the serial Neo Geo Pocket link and embedded browser are unavailable, and missing library routines are logged stubs. MiSTer docs acknowledge some transparency-sorting pixel differences; C audio modes on handhelds and other hosts can be about 1 ms early. The candidate's full-speed New 3DS and Steam-device claims remain promotional/project reports, without an independent platform matrix. Pinned docs were read, not the entire implementation; no game, SDK, build or port was downloaded, installed or run. Status is unverified; REA is unmentioned.

Sealed candidate: 65 likes, 1,550 views, 7 reposts, 0 replies. Neither later engagement nor repository existence verifies matching or completed ports.

## Sources

- [Candidate introduction of CvS2 v0.0.1, Claude use and five-platform ports, November 26, 2026 at 16:01:36 Beijing time](https://x.com/i/status/2125862523215692261)
- [Supplementary pinned root README: Claude disclosure, three-version matching and SDK/disc-data reuse; committed November 26, 2026 at 16:49:05 Beijing time](https://github.com/gibletto/cvs2-naomi-dc/blob/e3408908e9e9af696bada01e7281a5ac296282ef/README.md)
- [Port documentation at the same supplementary commit: platforms, host layers and audiovisual/network limits](https://github.com/gibletto/cvs2-naomi-dc/blob/e3408908e9e9af696bada01e7281a5ac296282ef/ports/README.md)

[中文](../cvs2-naomi-dc-claude-decompilation-native-ports.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
