# Native Mario Kart World on PC: Claude writes most code, but AArch64-to-C is not original-source recovery

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-14
Stage: In progress

At 16:30:11 Beijing time on November 14, 2026, yibie's three-project candidate names Mario Kart World, crediting Claude with most of the port and describing AArch64 translated to C ahead of time without an interpreter or JIT. The public list identifies adriadam10/mkw-recomp. Its README was read at c06721d, dated November 14, 2026 at 08:57:37 UTC, later than the candidate but within this window. It is supplementary evidence, not another candidate.

The goal is statically recompiling Nintendo Switch 2's Mario Kart World 1.0.0/1.8.0 for Linux and Windows. Documentation says CPU code becomes C ahead of time, with Linux also supporting AArch64; NVN2 is reimplemented over Vulkan, SM86 shaders become SPIR-V offline, and some Nintendo SDK functions are replaced by symbol. This is machine-code translation and host compatibility, not recovery of the original developers' C. It inherits TotK Recomp and community platform/shader research rather than Claude independently discovering the platform from scratch.

The author credits Claude with most typing under human direction, about ten full-time days and 489 commits starting October 30, each reviewed, measured or tested, explicitly not one prompt and done. Performance changes use A/B comparisons within one run because separate runs can differ by 12 ms. Rendering fixes are compared with console images, shader changes are tested offline across 11,561 programs before game runs, and frame replay helps isolate issues. Numbers and workflow are project statements. This collection did not enumerate commits, read all tests or confirm every gate was enforced.

An internal November 12 status reports booting, menus and races on Linux/Windows x86-64, plus Linux AArch64 tested on an Adreno 740 handheld. Menu, shadow, movie-audio and some AMD-hang issues remain, and there is no online play. A November 9–11 table includes high-end GPUs at 60 fps and GTX 1650 SUPER at about 24 fps; selected 60 fps results do not imply smooth play on every device, and generated frames do not make game logic faster. Users supply the game; MIT and third-party terms grant no game-asset rights. This collection downloaded no target, built nothing and ran no races. REA is unmentioned; retained as in progress.

Shared sealed candidate: 2 likes, 259 views, 0 reposts, 1 reply. The 720 stars are a dated secondary snapshot; about ten days, 489 commits and 11,561 shaders are project counts.

## Sources

- [yibie's current-window three-project introduction: Mario Kart World, November 14, 2026 at 16:30:11 Beijing time](https://x.com/i/status/2121521061955244445)
- [Supplementary pinned mkw-recomp README: Claude method, performance and known issues, commit November 14, 2026 at 08:57:37 UTC](https://github.com/adriadam10/mkw-recomp/blob/c06721d1a8fcc8fab3b4532ec4ea6badc73c485e/README.md)

[中文](../mkw-recomp-claude-aarch64-c-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
