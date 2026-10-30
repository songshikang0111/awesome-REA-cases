# sh4vita: Claude/Codex-assisted static recompilation brings Silent Hill 4 PC to PS Vita

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

The candidate at 02:25:06 Beijing time on October 31, 2026 presents sh4vita, bringing Konami's Silent Hill 4: The Room from its GOG PC release to PS Vita. It credits Claude and Codex with reverse engineering and coding, the developer with real-Vita testing, and v1.0.1 with long-session crash fixes. Supplementary research located vallfrr/sh4vita and read its README at commit 386541b726538a50f2e3cdf48d5ac24b553d6239, dated 2026-10-30T09:57:00Z. This earlier material supplies project context and limits, not an additional window candidate.

The documented pipeline exports function lists with Ghidra, translates x86 functions to C with recomp/x86rec.py, then compiles them with a replacement Win32, Direct3D 8, DirectInput and DirectSound runtime. D3D8 uses vitaGL. A separate Rust sh4prep tool prepares the player's own game files. Claude and Codex are explicitly credited for research and coding; design decisions and all real-hardware validation are human work. REA is not claimed.

The README reports start-to-finish playability on hardware, 30fps logic and interpolated rendering toward 60fps when performance permits. Enemy-heavy subway scenes, the water prison and some late rooms remain CPU-limited and can fall below 30fps. First room entry can pause for about a second. Sessions exceeding an hour can still exhaust memory, lose textures or close the game. Continue stays greyed out, requiring Load, and light glow is disabled for speed. Thus the candidate's v1.0.1 fix is not presented as eliminating all long-session crashes or delivering constant 60fps.

Only Windows GOG '1.0 gog v5' files are supported, not other releases or PS2 files. A modified Vita, at least 4GB free and the user's own shader-compiler module are required. Project code is GPLv3; neither the game nor generated C is distributed with the repository, and GPL grants no rights to Konami assets. This collection only read public documentation: no game download, preparer execution, VPK installation, frame-rate measurement or independent playthrough occurred.

Candidate snapshot: 0 likes, 80 views, 0 reposts. Playthrough, frame rates and fixes are project/report claims, not independent reproduction.
Supplementary pinned commit 2026-10-30T09:57:00Z predates the window; long-session memory limits are retained.

## Sources

- [Candidate relays sh4vita, AI assistance and v1.0.1 fixes, October 31, 2026 at 02:25:06](https://x.com/i/status/2116234958109122747)
- [Supplementary: October 30 pinned README, method, AI credit and remaining hardware limits](https://github.com/vallfrr/sh4vita/blob/386541b726538a50f2e3cdf48d5ac24b553d6239/README.md)

[中文](../sh4vita-silent-hill4-claude-codex-static-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
