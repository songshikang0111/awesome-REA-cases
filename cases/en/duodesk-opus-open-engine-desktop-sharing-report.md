# DuoDesk: Opus adapts the open TwinDesk sharing engine, not verified TeamViewer reverse engineering

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-01
Stage: Needs verification

At 22:29:42 Beijing time on October 31, 2026, Movez (@0xMovez) reports building DuoDesk with Claude Code/Opus 5.5 for shared Windows PC/MacBook mouse, keyboard, clipboard and cross-screen files, also advertising old-laptop/tablet second displays, no account, no cloud and encryption. The headline claims TeamViewer/AnyDesk reverse engineering, but the steps begin by supplying an open-source screen-sharing engine unnamed at the time, reading its Windows, Mac, Linux, Android and native input-helper code, then rebranding roughly 370 files with 11 parallel agents. One agent decides what must not be renamed to retain pairing compatibility. Adapting existing open code is not recovery of every protocol from proprietary binaries.

The author describes tag-triggered GitHub Actions for .dmg, .exe, AppImage, .deb and .apk installers, with Mac builds on cloud Apple hardware. An initial cursor crossing stalled at the Windows edge; Opus reportedly read logs, found the cause and added explicit crossing-refusal logs. A test deployment also took down the live website, reportedly rolled back in 20 seconds before agents lost deployment permission. Two days, zero personally written lines and recovery time are author figures, without workflow runs or logs as evidence. At 23:49:46, the same project adds remote-app windows, phone calls/texts/notifications/camera bridging and Wi-Fi, USB and Bluetooth claims, without individual tests here.

At 23:57:01 on November 1, Ahmed Reza (@AhmedReza) replies to later Movez promotion, pointing out the repository describes an Aurora redesign of TwinDesk and the first step supplied an open engine. He asks for original-author credit rather than a reversing claim. The README of 0xCodez/DuoDesk was additionally read at pinned commit 50125ca0c4f73ab3253e739dd8a6ec9cf1a8444b, dated October 31 at 23:09:36 Beijing time, before this candidate window. Credits explicitly identify a fork of TwinDesk by Inuka Asith, GNU GPL v3.0 and a claim of retaining original copyright notices. Parts are also credited to MIT-licensed DeskPad. The repository metadata's Aurora description matches the comment; upstream attribution is no longer unknown.

The pinned README is supplementary evidence, not a new candidate or an audit of all renaming, license compliance or cross-platform features. Existing sources and ID are retained while correcting the earlier absence of an identified upstream. No video was watched, installer inspected, code audited or two-computer test run. Encryption/no-cloud claims are not security conclusions, and website rollback does not validate complete compatibility. Retained as an unverified AI-assisted open-engine adaptation report. REA is unspecified.

Earlier first candidate: 60 likes, 2,553 views, 1 repost; later: 8 likes, 365 views, 0 reposts. New critical candidate: 1 like, 7 views, 0 reposts.
11 agents, roughly 370 files, two days and 20 seconds are author reports, not measurements or validation here.
The pinned README confirms the stated fork attribution, not license-compliance, encryption or compatibility auditing.

## Sources

- [Movez's DuoDesk/Opus workflow and failure-repair report, October 31, 2026 at 22:29](https://x.com/i/status/2116538107017212194)
- [Later same-project phone bridging and connection claims, October 31, 2026 at 23:49](https://x.com/i/status/2116558255040180315)
- [Ahmed Reza identifies the TwinDesk redesign and original-author attribution, November 1, 2026](https://x.com/i/status/2116922467797139641)
- [Supplementary pinned DuoDesk README Credits, committed October 31, 2026, before the window](https://github.com/0xCodez/DuoDesk/blob/50125ca0c4f73ab3253e739dd8a6ec9cf1a8444b/README.md)

[中文](../duodesk-opus-open-engine-desktop-sharing-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
