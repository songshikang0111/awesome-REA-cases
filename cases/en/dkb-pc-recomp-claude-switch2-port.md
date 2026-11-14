# Donkey Kong Bananza PC: Claude-assisted static recompilation with GPU crashes and later-area defects still open

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-14
Stage: In progress

At 16:30:11 Beijing time on November 14, 2026, yibie's list update introduces three independent projects. This entry covers only Donkey Kong Bananza PC. The candidate cites an FAQ crediting coding agents with most code, checked through game runs and differential testing. Reading the public list identified Lucas-blip-png/dkb-pc-recomp, whose README was read at fac48bc, dated November 13, 2026 at 14:20:24 UTC, with an internal November 13 status date. It is earlier supplementary material, not a new candidate.

The goal is bringing Nintendo Switch 2's Donkey Kong Bananza to native Windows x86-64. Documentation describes translating ARM64 to C ahead of time and compiling it, without a runtime CPU emulator, while a Vulkan host answers NVN2 graphics calls. It builds on TotK Recomp and uses Eglantine's Ampere lowering and Ryujinx-related shader translation. Claude Code is credited with most code and documentation, with humans responsible for reading and running it, not discovering all platform knowledge from scratch.

The status table reports 180,061 functions lifted without unsupported instructions and passing Unicorn differential tests, and 4,820 shader stages translated for the first 3D scene. These are project checks, not full-game behavioral or visual equivalence. It reports play beyond the first level on recent NVIDIA cards but lists NVIDIA/AMD device-lost errors, RADV hangs, guest crashes in later areas, missing effects and heavy scenes below 60 fps. Project defaults reportedly improve one heavy scene from about 53 to 58 fps, leaving about a 0.45-second area-loading stall; these are not benchmarks here. An older FAQ only describes a hand-played first level on RTX 5060 Ti. Newer player reports in the same document should neither be ignored nor treated as a full playthrough.

Users supply version 1.0.0 or 3.2.0 data. Version 3.2.0 only reports booting and 150 seconds at 60 fps near the start, without a play test. Linux/macOS are previews; Apple Silicon is only checked through mode selection and lacks destructible terrain. No game assets are included; GPL and inherited MIT terms grant no Nintendo rights. This collection read documentation only, without obtaining games, building, running differential tests or testing GPUs. REA is unmentioned; retained as in progress.

Shared sealed candidate: 2 likes, 259 views, 0 reposts, 1 reply. The 957 stars are yibie's dated secondary snapshot, not performance or independent testing.

## Sources

- [yibie's current-window three-project introduction: Bananza, November 14, 2026 at 16:30:11 Beijing time](https://x.com/i/status/2121521061955244445)
- [Pre-window pinned DKB README: AI attribution, status and limits, commit November 13, 2026 at 14:20:24 UTC](https://github.com/Lucas-blip-png/dkb-pc-recomp/blob/fac48bcdc5ec0edd6296bc3672bdebb540d5958d/README.md)

[中文](../dkb-pc-recomp-claude-switch2-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
