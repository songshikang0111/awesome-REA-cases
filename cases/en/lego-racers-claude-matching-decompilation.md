# LEGO Racers: Claude-credited commits in a matching decompilation of the 1999 game

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-20
Stage: In progress

At 16:30:12 Beijing time on November 20, 2026, yibie's list update introduces isledecomp/racers as matching C reconstruction of the 1999 LEGO Racers, claiming 188 AI commit trailers across the latest 30 commits. Supplementary reading of the README and commits identifies an ongoing decompilation of LEGORacers.exe and GolDP.dll. It uses Visual C++ 6.0 and reccmp comparisons against original machine instructions to create a modifiable codebase for later ports, rather than rebuilding a game from screenshots.

Pinned commit 7675cebe85578e529d384bc3a5a47ac6163cb553 originally dates to November 13 at 23:38:41 Beijing time, before this window and supplementary only. Its merge message repeatedly credits Claude Fable 5.2 and reports BeamEntity::Draw improving from 72.41% to 100% and PlayerControls::UpdateSteering from 83.80% to 100%, alongside collision and rendering functions still below 100%. Attribution establishes AI participation in particular commits, not a whole-project share. The list author's 188-trailer count was not independently recalculated and is not 188 distinct commits.

The same-revision README says the main executable is almost fully decompiled and most of GolDP is done; the rebuilt game is playable but its software renderer does not work yet. This repository targets 32-bit Windows only. The modern cross-platform adaptation is a separate racers-portable project, not a completed result here. No compiler, game or reccmp check was run by this collection. Whole-file equality, playability and unique recovery of original source were not verified. REA is unmentioned; status remains in-progress.

Sealed candidate: 0 likes, 153 views, 0 reposts, 0 replies. The 112 stars and 188 trailers are reported snapshots, not independently recalculated.

## Sources

- [yibie's list update covering two game projects, November 20, 2026 at 16:30:12 Beijing time](https://x.com/i/status/2123695393049604396)
- [Supplement: project README at the pinned November 13 commit](https://github.com/isledecomp/racers/blob/7675cebe85578e529d384bc3a5a47ac6163cb553/README.md)
- [Supplement: Claude attribution and specific function-match improvements in the November 13 merge commit](https://github.com/isledecomp/racers/commit/7675cebe85578e529d384bc3a5a47ac6163cb553)

[中文](../lego-racers-claude-matching-decompilation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
