# Leonida's native GTA VI runtime: Claude-credited contributions, but the project explicitly cannot boot the game

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-23
Stage: In progress

At 11:27:26 Beijing time on November 23, 2026, lei'zi (@lis1091fu) introduces Leonida, saying work independent of the game executable is done, most PRs are co-authored by Claude, and playability might precede an official PC release. This is a secondary project introduction. Fastest-moving, the hardest part being over and the playability timeline are the poster's judgments, not acceptance results.

Supplementary reading covers ItsNotRexed/Leonida pinned at commit 3eb4410, dated 11:56:15 Beijing time (03:56:15 UTC) within the window. The README describes static recompilation of Xbox Series GTA VI: with x86-64 CPUs on both platforms, native code is loaded while console system software is reimplemented; precompiled RDNA2 shaders become Vulkan SPIR-V, and models, textures and audio come from the user's own copy. It explicitly says the repository contains no game, keys or executable, gives no acquisition instructions and neither decrypts nor bypasses protections. It requires an already-readable, personally owned Xbox Series 1.0.2.1 package. This records the design, not verification of package authenticity or lawful provenance.

The crucial limit is explicit: Early, the game does not boot, and story mode or any playability is No. The project reports 26,503 translated shaders and successful spirv-val runs at some revisions; these are project validation claims, not output-semantic or whole-game execution proof. The hand-maintained status table retains duplicate, partly conflicting older and newer rows, including wave64 counts and graphics coverage. They are not reconciled here into a defect-free metric. Small handwritten GPU tests do not validate the game's shader outputs. PE loading and import shims have run a stand-in executable, not the real game. D3D12-to-Vulkan, some shader behavior, ray tracing and model decoding retain gaps. Work independent of the executable being in place does not establish that all difficult work is complete.

The same pinned commit describes a static PE tool ranking model-hash lookup candidates and synthetic PE tests, with Co-Authored-By: Claude Opus 5.5. The commit message and changed filenames were read, not the entire patch. This supports AI involvement, not the proportion of PRs, autonomous model completion or every test passing. A newer HEAD dated 12:04:16 was inspected only for comparison; its post-window CI change is not used to upgrade the candidate's results. Sources use the within-window revision. Linked GPU and corpus validation records were not all read. No game, script or target code was run, assets downloaded or dependencies installed. REA is unmentioned; status remains in-progress.

November 23 sealed candidate: 8 likes, 490 views, 3 reposts, 0 replies. README results are project-reported; tests and the share of Claude-credited PRs were not checked here.

## Sources

- [lei'zi introduces Leonida and Claude involvement, November 23, 2026 at 11:27:26 Beijing time](https://x.com/i/status/2124706360621498437)
- [Supplementary pinned project README: design, no boot and testing limits; revision dated November 23, 2026 at 11:56:15 Beijing time](https://github.com/ItsNotRexed/Leonida/blob/3eb4410b8de7a6d28cb81557e7bca6de864fda56/README.md)
- [Supplementary within-window commit: static PE tool, synthetic tests and Claude Opus 5.5 coauthor credit, November 23, 2026 at 11:56:15 Beijing time](https://github.com/ItsNotRexed/Leonida/commit/3eb4410b8de7a6d28cb81557e7bca6de864fda56)

[中文](../leonida-gta6-xbox-native-runtime-ai-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
