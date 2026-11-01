# PE2PC: Snaity's Claude-assisted native Windows port builds on the existing Parasite Eve II decompilation

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-02
Stage: In progress

At 02:12:46 Beijing time on November 2, 2026, the candidate reports Snaity (Adriano Teodoro)'s PE2PC port of Square's 1999 PlayStation game Parasite Eve II to Windows. It builds on the existing decompilation by GabeRealB and contributors, not Claude independently recovering the entire game from scratch.

Supplementary public search found Snaity-CORE/pe2-pc-port. README commit f8b34d128694f950e0c827b898d163621be2ccc3 is dated 2026-11-01T07:54:36Z, or November 1 at 15:54:36 Beijing time, before the candidate. It describes compiling decompiled C natively for PC, with a project-specific C compatibility layer and Rust host replacing console graphics, sound, CD, controllers and memory cards, claiming no emulator or Sony code. Claude Code wrote much of the code, tools and documentation; Snaity set goals, reviewed changes, played and tested, compared against DuckStation and committed. AI assistance must not erase attribution to the decompilation authors.

The project reports both discs, audiovisuals, saves and controllers working on Windows, resolution up to eight times the original 320x240, sub-pixel vertices and perspective-correct textures. Game logic remains at 30 fps, with intermediate model frames presenting 60 fps. Camera-relative movement, remapping, filtering, HD text and experimental asset/translation mods are described, alongside raw .mcd save exchange with DuckStation. These are project features and testing claims, not this collection's completion, performance or latency tests. Nightly builds explicitly have only CI testing.

Users need their own USA SLUS-01042 and SLUS-01055 disc dumps in CHD/CUE form, Windows 10/11 and Vulkan or OpenGL 3.3. The repository says it contains no game data. CC0 for original code does not license Square assets, and fonts/libraries retain separate licenses. Only static reading occurred: no release, assets, dependency installation, build or game execution. REA is not mentioned.

Candidate snapshot: 50 likes, 1,004 views, 12 reposts. The README predates the candidate and is not another window candidate.
Sixty-fps presentation interpolates 30-fps game logic. No independent rebuild or two-disc completion test; nightly has only CI testing.

## Sources

- [Candidate: PE2PC port and Claude-assistance report, November 2, 2026](https://x.com/i/status/2116956628771873001)
- [Supplementary pinned README: native architecture, AI roles and testing limits, November 1, 2026](https://github.com/Snaity-CORE/pe2-pc-port/blob/f8b34d128694f950e0c827b898d163621be2ccc3/README.md)

[中文](../parasite-eve2-pe2pc-claude-native-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
