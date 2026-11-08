# Redivivus: agents read Diablo II databases and propose corrections to a C++ reconstruction

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-08
Stage: In progress

A resource roundup at 16:30:20 Beijing time on November 8, 2026 introduces jaenster/redivivus: agents propose names and types for Diablo II: Lord of Destruction 1.14d Ghidra databases through read-only MCP, with writes confined to the proposal layer. The aim is recovering the shipped Game.exe as buildable C++ for single-player study and preservation, not writing a similar game or connecting to Battle.net.

Supplementary README, CONTRIBUTING and BYTE-MATCHING were read at bb149dcad7fd53c59f6d0d1d305a0f8656263a5f, committed at 18:35:56 within the window. Most source is generated from Ghidra databases, so names, types, prototypes and calling conventions should be corrected through address-based evidence proposals that are checked and reviewed, not edits to generated files that regeneration overwrites. A Claude Code plugin is documented; other agents can read Windows and same-source Intel Mac databases too. Function discovery/boundary changes require human-handled issues; generator defects belong in ghidra-reconstruct. Read access is not unrestricted writing or unreviewed autonomous repair.

The pinned README reports database v2035, 22 module libraries, strict C++17 compilation and linking without undefined symbols, and one completed single-player playthrough on a Visual C++ 2005 build. With the original Visual C++ 2005 SP1 compiler, it reports 7,772/14,626 matching functions (53.1%) and 629,221/2,598,518 bytes in whole matching functions (24.21%). Excluding 625 recovered matching functions without direct references gives 7,147/14,626 (48.9%). Address fields are normalized by their referents: this is not a byte-identical whole EXE. Headline metrics exclude the C runtime, compiler-generated exception helpers and PKWARE library. All 464 files compiling for x64 does not establish playable x64 support; 1,114 pointer-width casts remain.

Known issues include missing NPC quest-news scrolling text and occasional crashes, although quests can advance. Battle.net is out of scope. Users need their own 1.14 installation; no game data is included. Credits acknowledge blizzhackers, D2MOO and other prior human research rather than assigning all recovery to AI. Supplementary docs were retrieved November 9; their pinned commit is later than the roundup but within this candidate window. Build, playthrough and matching remain project reports. No code, game or oracle was run or downloaded here. REA is not mentioned.

Sealed candidate: 1 like, 288 views, 0 reposts. The roundup's 65 stars is its snapshot, not validation.
53.1% is the project's function-match rate; 24.21% is coverage by bytes of whole matching functions, not whole-EXE identity. Not independently retested.

## Sources

- [Candidate: resource roundup on Redivivus and read-only proposals, November 8, 2026 at 16:30:20 Beijing time](https://x.com/i/status/2119346771860349404)
- [Supplementary README pinned to the November 8, 2026 18:35:56 in-window commit: build, playthrough and limits](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/README.md)
- [CONTRIBUTING at the same commit: read-only agent access, evidence hierarchy and proposal review](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/CONTRIBUTING.md)
- [BYTE-MATCHING at the same commit: address normalization, denominators and exclusions](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/BYTE-MATCHING.md)

[中文](../redivivus-diablo2-ghidra-agent-proposals.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
