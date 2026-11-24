# Displaying NES content through SNES: Kenta IDA asks Claude about FPGA and PPU bandwidth

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-24
Stage: In progress

At 16:11:38 Beijing time on November 24, 2026, Kenta IDA (@ciniml) tells PentliumEE (@7GHz) that the problem has been passed to Claude and awaits a result. A supplementary parent from 15:38:40 identifies the idea: use an FPGA to display NES/Famicom content through SNES/Super Famicom. The author is unfamiliar with both specifications and worries it might effectively become an NES emulator using SNES only for display. This differs from the author's earlier QSPI cartridge random-read timing investigation and is not merged into that hardware target.

A 16:09:30 reply warns that bandwidth into the SNES PPU, its picture processing unit, may be insufficient and considers vertical/horizontal blanking and interlacing. The participant speculates that 2bpp might allow full resolution but the NES color requirements might force 4bpp, explicitly without testing. At 16:13:04 the same participant suggests asking AI to find the video-transfer section in an external reference. These are participants' hypotheses and research suggestions, not measurements or an implemented design.

The thread establishes only Claude's involvement in investigation. No FPGA design, specific game, bandwidth budget, code or hardware demonstration was obtained. Compatibility, the correctness of every color-specification assumption and impossibility are not established. REA is unmentioned; neither a model nor hardware was exercised here.

Sealed candidate: 0 likes, 43 views, 0 reposts, 1 reply. The 2bpp/4bpp discussion is hypothetical, not a specification validated by this collection.

## Sources

- [Candidate: Kenta IDA passes the investigation to Claude, November 24, 2026 at 16:11:38 Beijing time](https://x.com/i/status/2125140272715813250)
- [Supplementary parent: FPGA and NES display through SNES, 15:38:40](https://x.com/i/status/2125131974184743418)
- [Supplementary reply: untested PPU bandwidth, blanking and color-depth hypotheses, 16:09:30](https://x.com/i/status/2125139735916286155)
- [Supplementary reply: suggested AI search for video-transfer documentation, 16:13:04](https://x.com/i/status/2125140630443860315)

[中文](../ciniml-claude-nes-on-snes-ppu-bandwidth-study.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
