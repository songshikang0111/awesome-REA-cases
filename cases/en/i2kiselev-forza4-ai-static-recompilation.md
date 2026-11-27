# Forza Motorsport 4: AI-assisted recompilation adds an Apple Silicon preview and bounded comparisons

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-27
Stage: In progress

At 19:44:22 Beijing time on October 29, 2026, The Gaming Emporium reports i2kiselev's Forza Motorsport 4 static recompilation. Pinned 0be771c6 documentation from 09:13:11Z that day already acknowledges AI-assisted code, scripts, documentation and game-binary reversing, without naming models or REA. The new November 27, 11:23:19 candidate again introduces 0.3.2, emphasizing experimental Apple Silicon support, music, audio/older-CPU improvements, DLC fixes and shader preparation. This review reads the README, performance and macOS guides at 160ef51f716ebc6f90692d368d68f3a820fcecfe, committed November 15 at 14:47:30Z. These are pre-window supplementary documents, not a November 27 release. The pinned body already says 0.3.3; the promoted version is not treated as the only current version.

ShiftGlue translates PowerPC code ahead of time to C++, compiled for Windows x86-64 or Mac ARM64. Graphics use Vulkan, via MoltenVK on Mac. The project builds on arcanite24's Pinyon Shift and ShiftGlue fork, crediting ReXGlue, Xenia and earlier fm4-recomp; inherited runtime/renderer work is not attributed to AI building everything from scratch. FM4-specific depth, camera and object motion feed DLSS/FSR 2/3; newer docs also list FSR 4, Xbox 360 career imports and mouse look, with project support for keyboard controls, graphics settings, Disc 2, DLC and Project Forza Plus 4.

The 5120×2880 maximum and 240 fps ceiling are not one test. The retained bounded 0.3.0 comparison uses a Ryzen 7 5700X3D, 32 GB DDR4-3600, RTX 4070 Ti SUPER 16 GB and Windows 10 Pro 22H2 at Bernese Alps against eleven AI cars, roughly twelve seconds per row, medians of three runs, Console preset and upscaling off. At 1x/2x/3x/4x, averages are 233/232/156/102 fps, versus 102/88/68/45 on the same PC with pinned Xenia Canary. Thus 5K is 102 fps. The project's 2.3–2.6× claim is not universal across tracks, GPUs or configurations. A 170 Hz display is distinct from rendering throughput; the Mac preview does not inherit Windows benchmark figures.

Older docs supported PAL/USA 1.0 only, reporting Expert Division and about thirty Event List races. New pinned docs report all four Disc 1 releases, including Europe/USA Rev 1 or 1.1, World Tour to Professional, about seventy Event List races, Free Play, Test Drive, Autovista, photo mode, garage, replays and saving, plus Xenia career imports and Project Forza Plus 4 tests on 1.0/Rev 1 discs. This is the developer's expanded reporting, not checks rerun here. Split screen, wheels and most AMD/Intel GPUs remain untested; Xbox LIVE/Kinect are unsupported, and Linux/wheels remain roadmap items.

The Mac guide requires M1 or newer and macOS 14 or newer. Contributors report vanilla Free Play tests on M1 Max and M3 with a 60 fps cap and one error-free Vulkan-validation run. An external-NTFS setup with a third-party driver reached the title in about nine seconds, with brief shader-compilation dips. The guide retains workarounds for DB9 roof geometry and memory-check issues, and disables precompiled headers after a Clang 21 crash without a full subsequent setup retest. macOS 14 itself, Project Forza Plus 4 on Mac and FSR 2/3 race image quality still require validation. Build receipts establish neither gameplay checks nor byte-identical results across toolchains.

Users must supply supported, legally obtained discs and build locally; game code, assets and prebuilt games are not distributed. Roughly ten minutes for initial Windows setup is the project's estimate. These are developer documents and secondary reporting, not independent performance measurements. No installation, game download, target tests or recompilation was performed here.

Older sealed candidate: 1 like, 81 views, 0 reposts. This window: 0 likes, 81 views, 0 reposts, 0 replies. Retrieval-time engagement does not replace snapshots.
Project Windows single-PC short-race medians of three runs: 5K at 102 fps, not 5K at 240 fps or Mac performance. Not independently rerun.
Experimental; supported Disc 1 required. New docs include Rev 1 and a Mac preview, without comprehensive split-screen, wheel, most-GPU or actual macOS 14 validation.

## Sources

- [The Gaming Emporium reports FM4 recompilation and AI assistance, October 29, 2026](https://x.com/i/status/2115771724390178926)
- [Supplementary: pinned FM4 README, commit dated October 29, 2026, 09:13:11Z](https://github.com/i2kiselev/fm4-static-recomp/blob/0be771c68af81af5d74ca2e2c6284ec6b6642207/README.md)
- [Supplementary: same-commit test scope, environment and Xenia comparison](https://github.com/i2kiselev/fm4-static-recomp/blob/0be771c68af81af5d74ca2e2c6284ec6b6642207/guide/performance.md)
- [Current candidate introduces 0.3.2 and a Mac preview, November 27, 2026 at 11:23:19 Beijing time](https://x.com/i/status/2126154875775902054)
- [Pre-window pinned README: 0.3.3, AI disclosure and Rev 1, November 15, 2026 at 14:47:30Z commit](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/README.md)
- [Same pinned commit's performance conditions and expanded offline checks](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/guide/performance.md)
- [Same pinned commit's Apple Silicon tests and unvalidated scope](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/guide/macos.md)

[中文](../i2kiselev-forza4-ai-static-recompilation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
