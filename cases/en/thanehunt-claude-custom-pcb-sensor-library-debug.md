# Debugging custom-PCB firmware: Thane Hunt credits Claude with sensor-library and missing-DRDY research

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: Related project

At 03:01:52 Beijing time on November 11, 2026, Thane Hunt (@thanehunt) describes uploading a custom PCB's PDF schematic to Claude after receiving the board. LEDs, switches, Bluetooth, profiles and environment reportedly worked about twenty minutes later, followed thirty minutes later by Bluetooth OTA. The author says every firmware line was reviewed and Claude also identified slightly undervolted but functioning external flash. Timings and operation are author reports, not measurements here.

Beyond new firmware generation, the post says Claude found established libraries for the digital sensors and discovered bugs in two libraries authored by tier-one silicon companies. It specifically describes optimizing a state machine not to wait indefinitely for an ST DRDY signal that may fail to appear every 20,000–50,000 reads. This gives existing-library/device behavior as an AI-assisted understanding and debugging target. Chip/library names, patches and bus traces are absent, so protocol reversal or vendor confirmation is not established.

Full-text retrieval retains the author's 'put tests,' load tests and torture tests without silently correcting the first test category. Two weeks is a hypothetical manual-work estimate, not a controlled comparison. The author also urges caution for critical systems. No public board name, firmware, model revision or replayable records are supplied. This collection connected or flashed no board and ran no tests. REA is not named; included as a related device-debugging project, not a validated complete reversal.

Sealed snapshot: 1 like, 17 views, 0 reposts. Twenty minutes, another thirty minutes, two libraries and 20,000–50,000 reads are not independently verified.

## Sources

- [Candidate and full-text retrieval: Thane Hunt's PCB bring-up, sensor-library and DRDY debugging account, November 11, 2026 at 03:01:52 Beijing time](https://x.com/i/status/2120230477818966507)

[中文](../thanehunt-claude-custom-pcb-sensor-library-debug.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
