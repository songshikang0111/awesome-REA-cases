# DX RUST: a Rust/Bevy Deus Ex reimplementation still awaiting full-playthrough testing

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-01
Stage: In progress

At 08:15:55 Beijing time on November 1, 2026, the candidate introduces Grissyelda's DX RUST, a from-scratch Rust/Bevy reimplementation of Ion Storm's 2000 Deus Ex. It reads maps, textures, sounds, conversations and class defaults from the user's GOTY installation rather than merely running the old engine through a compatibility layer. The post advertises version 0.10.0, 73 maps, three endings and Windows/Linux/Steam Deck support, calling AI involvement heavy but unquantified.

Supplementary reading inspected README and commit metadata at 5ca15b0c68141a0b53ef7baac9d91fd96f7c570d, dated November 1 at 01:58:17 UTC, or 09:58:17 Beijing time: later than the candidate but within the window, used only as primary-source context. The README says the whole game is implemented and describes 83 map files, a different scope from the candidate's 73 maps; neither a conversion nor a confirmed map total is inferred. It documents original rules by default, optional modern graphics, controller/DualSense features, mod support and separate resource-reading modules. It also lists a full playthrough, performance work, Steam Deck tuning and save round-trip tests on every map as unfinished pre-1.0 work. Implemented does not mean campaign acceptance testing has passed.

The commit author is Claude, its message credits Claude Opus 5.5 as co-author, and GitHub's verification flag is true. It covers shadows, skeletal characters, coat cloth and mod compatibility. This supports AI involvement in that commit, not autonomous authorship of the entire project or functional correctness. The README licenses its own code GPL-3.0-or-later and requires separately supplied game/mod files. Its approximately 32-to-47-fps RTX 3050 Modern-mode figure is also a project report. Only documentation and commit metadata were read here; no build, execution, timing, asset-distribution audit or complete playthrough occurred.

Candidate snapshot: 11 likes, 660 views, 1 repost. Supplementary documentation postdates the candidate and is not another candidate.
73 maps and 83 map files are different source scopes; campaign and performance claims were not independently tested.

## Sources

- [Candidate report of DX RUST and AI involvement, November 1, 2026](https://x.com/i/status/2116685634307760281)
- [Supplementary pinned November 1, 09:58 README: map-file scope and remaining tests](https://github.com/Grissyelda/dx-rust/blob/5ca15b0c68141a0b53ef7baac9d91fd96f7c570d/README.md)
- [Supplementary same-revision Claude-authored repair commit and verification metadata](https://github.com/Grissyelda/dx-rust/commit/5ca15b0c68141a0b53ef7baac9d91fd96f7c570d)

[中文](../dx-rust-deus-ex-bevy-ai-reimplementation-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
