# X6200 without returning to stock Linux: Claude-assisted reconstruction of Xiegu's base updater merges into OpenX6X00

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-16
Stage: Needs verification

At 02:37:52 Beijing time on November 16, 2026, KF (@d0tslash) highlights a Claude-assisted open-source contribution, OpenX6X00 PR259. The Xiegu X6200 is a transceiver and OpenX6X00 a third-party UI/system project. Updating the base board responsible for DSP, RF, power and keying previously required returning to Xiegu's system and swapping cards. The goal is reproducing the stock updater in the alternative system, not breaking firmware signatures.

Supplementary reading covers Guru-RF/OpenX6X00 PR259, created November 13 at 18:55:41 UTC before this window, merged November 15 at 18:25:42 UTC (November 16 at 02:25:42 Beijing time), and closed when retrieved. Author MAVProxyUser reports disassembling Xiegu app 1.0.8's UPGRADE path, following its worker, handshakes, transfer and CRC, then writing a C writer, Python streaming extractor, GUI and SSH paths. The PR ends with Generated with Claude Code. The base bootloader itself decrypts official .xgf files; no key acquisition is needed and the PR distributes no Xiegu firmware. REA is unmentioned, and not every function-level finding is attributed to Claude acting independently.

The documentation reports CRC comparisons on 2,000 random packets, SHA/file-selection tests and simulated-base success/failure paths. Check-runs for head 9612ae8522ce1b57383614d44d588be0317cd1ad return one test job completed/success at 04:59:02 UTC on November 15. This is a project CI record, not a rerun or hardware certification by this collection. The author also reports three writes on one X6200 in their fork on November 13: 1.0.7 to 1.0.8, rollback and upgrade again, with transfers of 32.4, 27.9 and 32.4 seconds and calibration retained. Streaming extraction reportedly finished after reading 255 MB of a 371 MB zip, in 272 seconds using 68 MB memory. These measurements were not independently repeated.

Explicit limits include no X6100 support and no base-flash readback, hence no backup of the running firmware. Post-erase recovery follows the design but has not been validated against an actual failed write. The author tested at 11.8 V with the battery installed, contrary to the stock power conditions quoted in the documentation; this is not a flashing recommendation. Related gdyuldin/x6200_gui PR15, created November 13, ports the same writer but explicitly has not run on that GUI's image on hardware. It is supplementary background, not a separate project or new candidate.

This collection read only PRs, API status and CI records. It executed no downloaded code or target tests, installed no dependencies, downloaded no stock firmware and connected no radio. A merge and passing CI do not establish universally safe upgrades; hardware results remain unverified here.

Sealed candidate: 1 like, 101 views, 0 reposts, 0 replies. Three November 13 writes are author tests on one radio, not three devices.
The merge state and one successful check on the pinned head were confirmed through API reads; one-unit power conditions, no flash readback and untested recovery remain explicit.

## Sources

- [KF highlights Claude-assisted OpenX6X00 PR259, November 16, 2026 at 02:37:52 Beijing time](https://x.com/i/status/2122036376723951618)
- [Primary PR259: created November 13, merged November 16, 2026 at 02:25:42 Beijing time; stock procedure and author's single-radio tests](https://github.com/Guru-RF/OpenX6X00/pull/259)
- [Project test success on the pinned head, completed November 15, 2026 at 04:59:02 UTC; not rerun here](https://github.com/Guru-RF/OpenX6X00/actions/runs/43678985278/job/132705273774)
- [Pre-window related PR15: same-writer port, created November 13, 2026; target GUI image not tested on hardware](https://github.com/gdyuldin/x6200_gui/pull/15)

[中文](../x6200-claude-base-firmware-upgrade-reimplementation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
