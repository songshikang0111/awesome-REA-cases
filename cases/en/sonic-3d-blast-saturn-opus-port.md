# OpenSpindrift: Saturn Sonic 3D Blast byte-matching decompilation and a native port

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-21
Stage: In progress

On October 16, @TheOneMrMatt confirmed Opus accelerated byte-matching decompilation and said an AI disclosure had been removed because of anti-AI reactions. Historical updates identify Saturn Sonic 3D Blast: July research used SH2 code and frame-by-frame state from a custom emulator; on August 3 the author reported recreating a Hitachi compiler environment with Claude Code, recovering the SSSS.BIN Special Stage engine as C and handwritten assembly with byte matching, while three other executables were blocked by a particular GCC environment. On September 26 they reported 100% decompilation, with regional versions, documentation and porting still required. The October 16, 06:04 update describes a native C/SDL PC port with software rendering and OpenGL presentation, widescreen and Special Stage interpolation, but edge garbage and polygon seams remained. The first release was then planned for November 20 with user-supplied US/EU/JP disc files. At 12:26 the author clarified this was not static recompilation but a native port from claimed fully byte-exact, documented decompiled code. Months versus hypothetical manual years is retrospective estimation, not controlled labor measurement. October 20 evidence about four executables and Fable/Opus remains in metadata.

At 08:12:33 Beijing time on November 20, 2026, the same author, Mr. Matt (@TheOneMrMatt), says he has over twenty years of coding, engine and manual reversing experience and used agentic AI to decompile Saturn binaries from the beginning, aiming for months rather than years. He calls the port essentially a 1:1 translation with enhancements, all game logic native without emulation, running well even on Intel Atom netbooks from 2008, and extensively human-reviewed and tested. This adds author-reported process and named older hardware, not collection-confirmed 1:1 functionality, frame rates, byte matching or complete test coverage. The project was previously identified through author and Saturn context without obtaining that reply's parent or full thread.

At 23:30:01 on November 21, this window's candidate, David24 (@Davis24X), replies in Mr. Matt's release-announcement thread, saying reversing the original was AI-assisted but all code was reviewed and fixed by hand, with new menus and other elements also written manually. David24 also claims Windows XP operation. David24's developer role is not established, so this is not attributed directly to Mr. Matt as a technical guarantee; XP compatibility was not tested.

To identify the target, the pre-window original announcement at 08:57:39 on November 21 was read as supplementary evidence. Mr. Matt says OpenSpindrift's first release, 2026.11.20, is available: a native port built from the Saturn version's decompiled code, currently supporting Windows, Linux and Android. Source cleanup was ongoing with publication hoped for soon, documentation was lacking, and GitHub CI/CD was not wired up. The first release was still rough, some enhancements were omitted, and further updates were planned. Users must place their own Saturn game CHD in assets; the Saturn/Genesis toggle additionally requires their own Genesis ROM. The version number is not the Beijing-time post date, and this announcement is not a new candidate in the window.

The earlier unconfirmed release is corrected to an author-announced first release, not a release package downloaded and validated by this collection. No new source, matching output or test matrix was reviewed, no game was run, and resolution of earlier visual defects remains unknown. In-progress status reflects continuing development and verification limits. Release reporting, human-review claims and independent reproduction are attributed separately; AI assistance is not rewritten as autonomous completion.

Earlier statement candidate snapshot: 0 likes, 14 views; supplementary originals range from July to October 16 and are not presented as new achievements.
October 16 candidate snapshot for the 12:26 statement: 1 like, 147 views; months versus hypothetical manual years is author-reported.
Separate review of the author's October 20, 08:36 reply: Claude Code's Fable and Opus reportedly recovered four Saturn executables as readable C with some SH2 assembly, claimed 100% byte-matched, and the native PC port builds on that code. Low CPU/memory requirements remain an expectation without hardware measurements or new matching outputs. Not independently rerun here; candidate snapshot: 0 likes, 86 views.
November 21, 23:30 candidate snapshot: 0 likes, 11 views, 0 reposts, 0 replies. David24's human-review and XP claims are not independently verified. The pre-window first-release announcement is used only to identify the project and correct release status.

## Sources

- [Author confirmation of Opus involvement](https://x.com/i/status/2110939629516186067)
- [August 3 historical update on Claude-built compiler tooling](https://x.com/i/status/2084352916253762001)
- [September 26 decompilation progress report](https://x.com/i/status/2103692693037826484)
- [October 16 06:04 PC-port update as supplementary background](https://x.com/i/status/2110854238989582709)
- [July 16 SH2 and emulator investigation approach](https://x.com/i/status/2077571522248732787)
- [October 16 12:26: author clarifies native port and months of AI-assisted decompilation](https://x.com/i/status/2110950579254264278)
- [Separately reviewed October 20, 08:36 reply: four executables, Fable and Opus](https://x.com/i/status/2112342047525118198)
- [Mr. Matt confirms AI from the start, human tests and Atom-netbook play, November 20, 2026 at 08:12:33 Beijing time](https://x.com/i/status/2123570152432411080)
- [David24 on AI assistance, human review and XP, November 21, 2026 at 23:30:01 Beijing time](https://x.com/i/status/2124163429954924817)
- [Pre-window supplementary original: Mr. Matt announces OpenSpindrift's first release, November 21, 2026 at 08:57:39 Beijing time](https://x.com/i/status/2123943892596978114)

[中文](../sonic-3d-blast-saturn-opus-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
