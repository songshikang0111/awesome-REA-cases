# Mario Kart 64 native PS3 port: existing decompilation, Claude collaboration and author hardware testing

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-11
Stage: In progress

At 16:30:17 Beijing time on November 11, 2026, yibie's roundup introduces Mario Kart 64 on PS3, describing an existing decompilation running on PSL1GHT, no bundled game assets, runtime loading from the user's ROM and named AI disclosure. This differs from Mario Kart Wii, web MK64 and MK8 Deluxe projects.

Supplementary reading covers the entire README at stingziz0u/mk64-ps3 commit 32602e5f01dd71820e1174ebde7ff10351ab4fe8, dated November 11 at 10:44:01 Beijing time, before this window. It is supporting documentation, not a new candidate. The project explicitly builds on the existing n64decomp/mk64 decompilation; upstream manual work is not reassigned to AI from scratch. Its disclosure says the author collaborated with Claude in real time over many sessions and personally did all testing/debugging on real hardware. This is a project report, not this collection's hardware reproduction. REA is unmentioned.

Documented features include the original audio engine at 48 kHz, 720p scaling, 4:3/16:9, one to four DualShock 3 players, 30 FPS or interpolated 60 FPS, and Controller Pak emulation for Time Trials ghosts. Interpolation is not a measurement of stable 60-FPS native game logic. Data-only mods are supported by rebuilding 599 tables from the ROM; code/assembly hacks are unsupported, about 190 read-only tables are not rebuilt, and heavily rearranged ROMs may load but fail. A qemu PowerPC host test is described without test outputs inspected here. A legally obtained USA ROM is required. No game assets were downloaded and no PKG was built or run by this collection.

Whole roundup: 2 likes, 249 views, 0 reposts. Seven stars and 953 files are relayed claims, not independently counted or measures of game completion.

## Sources

- [yibie's MK64 PS3 account, November 11, 2026 at 16:30:17 Beijing time](https://x.com/i/status/2120433924434452690)
- [Supplementary README and AI disclosure, pinned to a pre-window November 11, 2026 10:44:01 Beijing-time commit](https://github.com/stingziz0u/mk64-ps3/blob/32602e5f01dd71820e1174ebde7ff10351ab4fe8/README.md)

[中文](../mario-kart64-ps3-psl1ght-ai-port-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
