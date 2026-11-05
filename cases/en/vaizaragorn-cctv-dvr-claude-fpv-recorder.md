# An old CCTV DVR as an FPV recorder: Claude, UART and Ghidra MCP research reports

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-05
Stage: In progress

At 20:10:46 Beijing time on November 5, 2026, whyamas relays @vaizaragorn turning an old 2011 CCTV DVR into an FPV ground station with new firmware. A DVR records surveillance footage; FPV means first-person flight video. The developer needed a ground-station recorder, could not easily buy a local module and tried inexpensive old hardware. The 2011 date and firmware 'from scratch' claim come from the current-window retelling, not a verified hardware history.

To establish AI involvement, supplementary research reads the author's July 22–25, 2026 posts, with dates in UTC and outside this window. On July 22 the author describes an unpopulated UART, terminal access over USB/TTL and asking Claude to study, dump and modify the device. On July 23 the author reports studying key components through Ghidra MCP, creating a toolchain and having Claude build a modern web UI. Custom programs then disappeared on reboot; permanent flashing was not yet done. On July 25 the author reports custom firmware for analog FPV AV recording, live viewing and media playback, with the web UI hosted externally to conserve resources.

The author explicitly says only about 50MB of 128MB RAM is usable and recording bitrate is limited, making fast-motion footage poor, and plans a better board. The original posts support AI participation and firmware modification, not a complete from-scratch replacement of every firmware component. The later ground-station description is not upgraded into a mature low-latency flight system. Firmware source, exact hardware model and recording comparisons were not obtained. No UART connection, flashing or code execution was performed here. REA is unconfirmed.

Current-window sealed snapshot: 1 like, 17 views, 0 reposts. July material is supplementary historical evidence, not a newly released project or independent testing.

## Sources

- [Current-window whyamas DVR-to-FPV retelling, November 5, 2026 at 20:10:46](https://x.com/i/status/2118315081763324306)
- [Supplementary author post: UART and Claude plan, July 22, 2026 UTC](https://x.com/i/status/2080052847182311577)
- [Supplementary author post: Ghidra MCP and toolchain, July 23, 2026 UTC](https://x.com/i/status/2080262141425103162)
- [Supplementary author post: firmware uses and hardware limits, July 25, 2026 UTC](https://x.com/i/status/2081033505736110540)

[中文](../vaizaragorn-cctv-dvr-claude-fpv-recorder.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
