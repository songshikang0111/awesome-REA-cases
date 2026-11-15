# PocketPort Anything: an AI-assisted 3DS porting research framework, not a universal game converter

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-15
Stage: In progress

At 16:30:12 Beijing time on November 15, 2026, yibie (@yibie) introduces PocketPort Anything in a catalog update, emphasizing that 'anything' describes investigation scope, not promised compatibility. The Console skill in the same post is already cataloged here. PocketPort is a separate AI-assisted research and engineering framework targeting Nintendo 3DS, not a renamed PS2 toolkit; other directories in the post are not treated as new game results.

The linked catalog identifies Alexispher/pocketport-anything. Supplementary research read its README at 9a7d588a2574683ca33f9c4717d472193916f986, committed November 15, 2026 at 02:17:03 UTC, before this window. It asks agents such as Claude Code and Codex to identify engines, formats and existing source ports, then choose reconstruction, adaptation or an explicitly labeled alternative and retain build/validation evidence. Documented implemented scope includes file inventories, read-only NUP metadata, a limited uint32 intermediate representation translated to C99 with host semantic comparisons, and the original Star Catcher C runtime. It is not a general ARM64, x86 or MIPS machine-code translator.

The documentation reports cross-compilation of dual-screen Star Catcher and a limited Skyrim 3D viewer, while same-build dual-screen pixels, Azahar and physical 3DS execution remain unvalidated. The Skyrim path covers limited BSA/TES5/NIF static-resource and geometry work, not full worlds, collision or original gameplay. Appended source-engineering updates mention investigations of The Legend of Edgar and L'Abbaye des Morts sources, not complete playable 3DS ports. Older roadmap sections coexist with later implementation notes: neither all pending work nor host testing should be promoted to implemented features or hardware proof.

The project states MIT licensing and no commercial game-data distribution. NUP here is an emulator-specific container; the extension does not prove an official package or 3DS compatibility. Documentation notes a v0.3.1 archive versus some 0.2.0 package metadata; this discrepancy is preserved rather than repaired for the author. REA appears only as a research reference, not proof of runtime REA use. This collection installed no dependencies, executed no target, built nothing and reran no project tests. Included as an in-progress research framework.

Whole candidate post: 8 likes, 533 views, 0 reposts, 7 replies; not project-specific engagement.
v0.3.1 versus 0.2.0 is a documented metadata discrepancy. No validated count of complete commercial-game ports.

## Sources

- [yibie introduces PocketPort, TA Reborn and other projects, November 15, 2026 at 16:30:12 Beijing time](https://x.com/i/status/2121883453767688434)
- [Pre-window pinned PocketPort README: methodology, implementation and validation limits, committed November 15, 2026 at 02:17:03 UTC](https://github.com/Alexispher/pocketport-anything/blob/9a7d588a2574683ca33f9c4717d472193916f986/README.md)

[中文](../pocketport-anything-ai-3ds-porting-research-framework.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
