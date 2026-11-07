# Famicom cartridge timing: Kenta IDA asks Claude whether QSPI random reads can respond in time

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-07
Stage: In progress

At 07:11:32 Beijing time on November 7, 2026, Kenta IDA (@ciniml) says they do not know Famicom memory-access timing and have begun investigating—or rather, Claude has. The author describes QSPI Quad IO sending a command, address in four-bit chunks, dummy cycles and then four-bit data, so even an eight-bit read may take appreciable time. The purpose is assessing whether QSPI Flash can respond to the Famicom cartridge bus.

Supplementary parents from 07:04:22 and 07:08:46 that day identify the context: burst throughput may suffice, but random reads must wait for the console address, send it to Flash and receive the first data before driving cartridge data lines, making latency tight. These parents are context within the window, not supplied candidates. No Flash model, clock, cache/bridge design, timing diagram, numeric budget or logic-analyzer measurement is supplied. A question is not proof of incompatibility or an implemented cartridge. Whether Claude searched documentation or analyzed hardware is unspecified, and REA use is unconfirmed. No code or device was exercised here.

Sealed candidate: 3 likes, 153 views, 0 reposts. Four-bit and eight-bit figures describe interface granularity, not measured latency.

## Sources

- [Candidate: Claude investigates Famicom timing, November 7, 2026 at 07:11:32 Beijing time](https://x.com/i/status/2118843758083285166)
- [Supplementary parent: QSPI random-access latency question, November 7, 2026 at 07:04:22](https://x.com/i/status/2118841954712908026)
- [Supplementary thread: address availability to data-line response, November 7, 2026 at 07:08:46](https://x.com/i/status/2118843058687283330)

[中文](../ciniml-claude-famicom-qspi-memory-timing-study.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
