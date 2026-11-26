# Rockbox on a $9 SL6801 player: relayed AI firmware research and a low-memory port

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-26
Stage: Needs verification

A short post at 04:58:06 Beijing time on November 26, 2026 says a developer used Claude to port Rockbox to an undocumented $9 AliExpress MP3 player, citing 160 HN points and 70 comments without a checked HN page. At 05:12:40, Embedded Systems (@embedsys) adds a Smartlink SL6801 with two 192 MHz Cortex-M4 cores, 512 KiB SRAM, 2 MB flash and uncached XIP. Codecs and plugins reportedly share a 128 KiB arena, so starting a plugin stops music; profiled hot loops move into SRAM. The claimed 2 MiB smallest previous target is the post's comparison, not a checked history of Rockbox targets.

The reported method uses ghidra-mcp on stock FreeRTOS firmware, a webcam for the screen, line-in for audio, a bidirectional USB development shell for injected keys and screenshots, and hours of Python stress testing. Drivers were reportedly redone with a Ghidra researcher, referee and implementer. The account says the case was never opened and the author only glanced at code, calling it 100% vibecoded, while crediting ilyakurdyukov for ROM download-mode discovery and the flashing tool. This implies neither zero human participation nor a legally assured clean room. Claimed upstream bugs lack linked submissions and reproduction records.

Supplementary public GitHub search located jaydens-tasty-slop/rockbox, described as a YP3 (SL6801) port. Its pinned master commit 822b9f5e999122bc25738fc9746bb7a17bb48fa6 dates to November 22 at 09:01:21 Beijing time, before this window. Only repository identity, commit and root listing were checked; implementation was not reviewed and no root README was found. Repository existence cannot validate all reported specifications or outcomes. This is distinct from the existing unimplemented idea of rewriting a daughter's $10 player firmware. No dependencies were installed, firmware downloaded, code run or device flashed. REA is unmentioned.

Sealed candidates respectively: 0 likes/11 views/0 reposts/1 reply and 8 likes/525 views/2 reposts/2 replies. HN engagement is only relayed by the short post.

## Sources

- [Claude/$9 Rockbox-port short report, November 26, 2026 at 04:58:06 Beijing time](https://x.com/i/status/2125695546543243614)
- [Embedded Systems adds SL6801 details, research method and maintenance concerns, November 26, 2026 at 05:12:40 Beijing time](https://x.com/i/status/2125699211169509405)
- [Supplementary located YP3/SL6801 repository pinned to November 22, 2026; implementation not reviewed](https://github.com/jaydens-tasty-slop/rockbox/tree/822b9f5e999122bc25738fc9746bb7a17bb48fa6)

[中文](../rockbox-sl6801-nine-dollar-player-ai-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
