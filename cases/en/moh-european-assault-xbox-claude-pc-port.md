# Medal of Honor: European Assault: Claude-assisted Xbox recompilation and an author-tested Windows port

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-01
Stage: In progress

At 07:32:17 Beijing time on November 1, 2026, The Gaming Emporium reports boodyandmustafa-create's Windows port of Medal of Honor: European Assault, a 2005 console WWII shooter. Supplementary reading inspected README, PROJECT_STORY.md and SOURCE.txt at commit d097881e242b2925589c3e6281dd88e1052bd602, dated October 31 at 16:16:33 UTC, or November 1 at 00:16:33 Beijing time. These are pre-window primary documents. They credit Claude Code with interactively doing most reversing and coding while the human author tests each change in the real game, not an unsupervised autonomous port.

The project uses xboxrecomp to translate the USA/NTSC-U DEFAULT.XBE function by function into C and compile x86-64 code, removing Xbox CPU emulation. Audio/video chips, memory layout and other hardware behavior still use xemu-derived emulation. The story reports optimizing an approximately 1.3 fps software renderer to 25–30 fps before translating draw commands into Direct3D 11. Native mouse support required finding actual stick-to-camera logic; widening the field of view also required consistent culling/LOD rather than one numeric tweak. Audio investigation reportedly compared a reference decode section by section and byte by byte, finding an 8-bit multiply translated into a wider operation that corrupted a lookup index. Further work corrected six-to-two-channel mixing and added a recovery guard for long-session audio-ring stalls. These are project accounts, not performance or differential tests by this collection.

The README identifies version 0.9.0-beta for 64-bit Windows 10/11, advertising widescreen, 4K, native mouse aiming, remapping, a launcher and partial Arabic support. Its English limitations say 60/90 fps is stable and 120–240 fps experimental, whereas its Arabic summary confirms only 60 fps. The 90 fps statement is not treated as a guarantee consistent across both languages. Long-session sound can still disappear; only magazine-size weapon mods are confirmed, sound replacement is not tested end to end, and Arabic subtitles remain partly untranslated or clipped.

SOURCE explicitly says the recompiled game and main port code are not open source, identifying only xemu-derived parts and a route to request relinking objects. Public GitHub documentation is not a full open-source rebuild. Users must supply USA game files; documentation says no assets are bundled, but releases were not downloaded to audit that claim. Personal noncommercial terms do not grant permission to redistribute EA's game. No tools were installed, game run or tests independently repeated. REA is not mentioned.

Candidate snapshot: 2 likes, 162 views, 1 repost; documentation only, port not executed here.
Pinned documents predate this window. Performance, audio repairs and stability are project reports; main code is not open source.

## Sources

- [The Gaming Emporium's MOH port report, November 1, 2026](https://x.com/i/status/2116674651480809567)
- [Supplementary pre-window pinned README: AI attribution, features and limits](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/README.md)
- [Supplementary pinned development story: human testing, rendering and audio diagnosis](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/PROJECT_STORY.md)
- [Supplementary pinned SOURCE statement: partial source only, main code not open source](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/SOURCE.txt)

[中文](../moh-european-assault-xbox-claude-pc-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
