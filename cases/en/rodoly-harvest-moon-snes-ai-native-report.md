# SNES Harvest Moon: RodoLy uses AI to recover readable C and offers a native PC beta

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: Analysis test

At 12:48:40 Beijing time on October 31, 2026, The Gaming Emporium (@McGroin83) reports RodoLy's C reconstruction and PC beta of 1996 SNES Harvest Moon, claiming verification of 778 routines and 45,176 instructions and provisionally calling AI usage heavy and human-supervised. This is not the existing PS1 Back to Nature case.

Supplementary reading used the complete README of RodoLy/HarvestMoonSnesDecomp at commit 54e7371118af81ba6c9a8b00dbd6b951a7d43099, dated October 30 at 07:50:50 Beijing time, before the candidate. The author says that after recompilation they wanted to understand a favorite game routine by routine and run it only on recovered C. They explicitly credit AI assistance under human direction, testing on their own PC and human decisions about what stays; no model or REA is identified. Names and memory maps build on ElisaS-Codes and DasK's HM-Decomp. The project counts 100% instruction/routine coverage and describes comparing 128KB WRAM including the stack, CPU and DMA registers, alongside randomized calls and scripted playthroughs. These are project-documentation claims, not reruns here or proof over every possible game state.

The native build calls recovered C directly rather than emulating the SNES CPU, but picture and sound chips still run in software. Documentation covers Windows x64/ARM64 and Linux; the Windows beta download contains source and a local build script, not a ready-to-play complete game. A legally obtained USA ROM is required. Options include 16:9, ten save-state slots, an HM64-style pause menu and farming beyond the Year 3 ending. Widescreen reverts to 4:3 at map edges, in small rooms and on the title screen, so it is not universal. Project code uses PolyForm Noncommercial; it does not license original game assets. No ROM download, dependency installation, game build or checker execution occurred here. Beta and project-test limitations remain explicit.

Candidate snapshot: 0 likes, 194 views, 0 reposts. 778, 45,176 and 100% are project figures, not independently verified.

## Sources

- [The Gaming Emporium's SNES Harvest Moon report, October 31, 2026](https://x.com/i/status/2116391886118121955)
- [Supplementary pinned README: AI disclosure, verification and native build, October 30, 2026](https://github.com/RodoLy/HarvestMoonSnesDecomp/blob/54e7371118af81ba6c9a8b00dbd6b951a7d43099/README.md)

[中文](../rodoly-harvest-moon-snes-ai-native-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
