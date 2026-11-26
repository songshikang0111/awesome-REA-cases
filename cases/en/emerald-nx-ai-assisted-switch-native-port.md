# Emerald NX: an AI-assisted native Switch port introduction, with first hardware boot still pending

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-27
Stage: In progress

At 01:12:01 Beijing time on November 27, 2026, The Gaming Emporium (@TheEmporium83) introduces eonlynx's Emerald NX v0.5.0: a native Switch port of Pokémon Emerald based on the pret/pokeemerald decompilation and existing Emerald 3DS/Android engines. The introducer says the developer confirmed extensive AI assistance. This is relayed attribution, without developer model sessions; pret's existing decompilation must not be credited to this AI-assisted port.

Supplementary reading pins the README and November 25, 2026 final audit to eonlynx/emerald-nx revision a64db5d03de9e430157753314bf21656d91b3904, committed November 26 at 15:03:49 UTC, before this window. The project describes libnx/GLES3, a two-stage NRO loader keeping addresses below 4 GiB, 720p handheld/1080p docked output, a single-screen touch layout, optional voxel scenes and ARM32/AArch64 save-layout checks. Voxel mode is off by default, much of the map and interiors remain flat, and local wireless is stubbed.

The main caveat is stronger than the introduction's release wording: the README explicitly says no console has run the final package and the first hardware test is pending. The audit reports a passing full AArch64 build/package, save-layout checks and thirteen reviewed overlay exceptions, not on-hardware verification of graphics, audio, save migration or the whole game. Features such as following Pokémon, the physical/special split and unlimited TMs are inherited, not independent inventions of this AI port. A lawful game source is required; generated pak files still contain game content even if they are not ROMs, so absence of a ROM does not authorize redistribution. Only documentation was read here; no game data, dependencies, build or execution were obtained. Status remains in-progress.

Sealed candidate: 19 likes, 813 views, 3 reposts, 0 replies. v0.5.0 follows the introduction; the AI model is unspecified.

## Sources

- [The Gaming Emporium's Emerald NX/AI introduction, November 27, 2026 at 01:12:01 Beijing time](https://x.com/i/status/2126001039723639201)
- [Pre-window pinned README: first hardware boot pending, committed November 26, 2026 at 15:03:49 UTC](https://github.com/eonlynx/emerald-nx/blob/a64db5d03de9e430157753314bf21656d91b3904/README.md)
- [Same-revision November 25 build/static audit, not tests rerun here](https://github.com/eonlynx/emerald-nx/blob/a64db5d03de9e430157753314bf21656d91b3904/switch_port/FINAL_AUDIT_2026-11-25.md)

[中文](../emerald-nx-ai-assisted-switch-native-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
