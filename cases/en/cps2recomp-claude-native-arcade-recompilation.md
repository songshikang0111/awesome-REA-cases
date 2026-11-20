# CPS-2 Recomp: Claude-credited native arcade recompilation with unresolved timing checks

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-20
Stage: In progress

At 16:30:12 Beijing time on November 20, 2026, yibie introduces tmcleroy/cps2recomp: Capcom CPS-2 programs translated into C++ and run on a machine implemented for the project, for macOS, Linux, Windows and Android, adding training and rollback play to fighting games. Supplementary reading of the README and ARCADE_ACCURACY at fcd63e519796b8a3948e3c946b1d5bb85c23ae1b also identifies some CPS-1 games. Its not-an-emulator label does not mean no hardware behavior is modeled: video, sound and board behavior are reconstructed. Users need their own named ROM revisions and required keys; the repository supplies no game data.

Supplementary commit ec0fdfff30132f02f7fd1bc0be6becd151fad140, dated November 20 at 15:14:56 Beijing time, credits Claude Opus 5.5 for timing-accuracy documentation. Earlier change f333656 also credits Claude and defaults to board waits and DMA timing after testers reported Hyper Fighting and Super Turbo running too fast. Both predate the strict 16:00 window: supplementary evidence of AI work and method, not new candidate posts.

The reference is jtcps2/jtcps1 simulated with Verilator, not a physical board. SFA2's earlier setting reportedly matched work RAM on 5,639 of 5,671 frames. Counting the DMA scheduler changes that to 5,634/5,671, with a fixed eleven-frame boot offset and approximately 0.16% per-frame DMA difference. Hyper Fighting's reported fight-speed difference is about 0.2% against a 10 MHz test reference; actual play uses 12 MHz. These are project results, not reruns by this collection.

The document explicitly retains lasting Vampire Savior divergence after about 2,000 frames, excluded RAM regions, incomplete picture and within-frame comparisons, a stubbed QSound reference, inexact timing in added modes, and a harness and input scripts still confined to the author's machine. The README's Arcade perfect option does not establish arcade perfection. This collection did not build the project, download ROMs, execute targets or independently test online play. Status remains in-progress; claims of playability or model comparisons do not establish all-game or physical-board equivalence.

Sealed candidate: 0 likes, 153 views, 0 reposts, 0 replies. The list's 201-star snapshot does not validate arcade accuracy.

## Sources

- [yibie introduces CPS-2 Recomp, November 20, 2026 at 16:30:12 Beijing time](https://x.com/i/status/2123695393049604396)
- [Supplement: README pinned to November 20 at 15:47:20 Beijing time](https://github.com/tmcleroy/cps2recomp/blob/fcd63e519796b8a3948e3c946b1d5bb85c23ae1b/README.md)
- [Same-revision ARCADE_ACCURACY: comparison methods, divergences and unpublished harness](https://github.com/tmcleroy/cps2recomp/blob/fcd63e519796b8a3948e3c946b1d5bb85c23ae1b/docs/ARCADE_ACCURACY.md)
- [Supplement: Claude-credited timing-accuracy documentation, November 20 at 15:14:56 Beijing time](https://github.com/tmcleroy/cps2recomp/commit/ec0fdfff30132f02f7fd1bc0be6becd151fad140)
- [Supplement: Claude-credited default board-timing fix, November 20 at 13:43:17 Beijing time](https://github.com/tmcleroy/cps2recomp/commit/f333656cf99d1794d2e072e357b31cd01adc06ce)

[中文](../cps2recomp-claude-native-arcade-recompilation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
