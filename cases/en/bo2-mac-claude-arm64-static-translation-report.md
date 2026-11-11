# bo2-mac: a report of Claude-assisted static translation of Black Ops II to an ARM64 Mac app

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-11
Stage: Needs verification

At 22:50:17 Beijing time on November 11, 2026, cryptopsihoz (@rimtoln) replies to vibelancer about native ARM BO2 and credits AI-assisted reversing. Supplementary reading of vibelancer's 22:41:10 thread root identifies bo2-mac, intended to play Call of Duty: Black Ops II on a 2020 M1 MacBook. It relays a developer's claim of building the tool with Claude Opus 5.5. This is context and secondary evidence for the candidate, not another candidate or a reproduction by this collection.

The account starts with three x86 Windows EXEs from the user's Steam copy: Ghidra lists functions, Remill v6.0.1 lifts to LLVM IR, custom passes optimize it, and clang -O2 produces ARM64. It claims roughly 150,000 functions and five Remill patches. A Win32 implementation, a 4GiB guest mapping, D3D11-to-Metal, 2,664 shaders through HLSLcc and XAudio2-to-CoreAudio provide runtime support. Despite promotional no-emulator/no-Wine-or-JIT wording, the account explicitly places some protection sequences and missed functions in a tiny Unicorn x86 VM. Entirely emulation-free execution is therefore not claimed here. Executing rather than bypassing protection, exact-Steam-build hashing and Mac ownership checks remain reported, not audited mechanisms.

On one M1, the report gives about 1 hour 45 minutes for conversion, roughly 4GB on disk, 720p-window campaign rates of 51–60fps, Zombies at 57–60fps across six maps and bot multiplayer at 53–60fps. Online play is absent, the project is beta and temperatures reportedly reach 111–116°C. Static Metal buffers allegedly reduce per-frame geometry uploads from 23–63MB to 3.5–5MB and raise multiplayer from 51.8 to 60fps. Thirteen quantified findings, roughly 1,100 advance predictions and about 200 retracted conclusions are also reported. All are secondary claims without sensor placement, repository, test logs or itemized records checked here. Other Macs, complete playthroughs and thermal safety are not established; prediction count is not accuracy.

The video was not watched; no game was downloaded, port built or protection code run. Redistribution authorization is unconfirmed. A legally obtained game is required, and the report's no-sharing statement is not treated as a legal determination. REA is unmentioned. Status remains unverified.

Sealed candidate: 0 likes, 26 views, 0 reposts. The supplementary root's 49 likes/477 views/1 repost is a separate retrieval snapshot, not the candidate's engagement. All performance figures are secondary reports.

## Sources

- [Candidate: rimtoln's native-ARM BO2/AI-reversing reply, November 11, 2026 at 22:50:17 Beijing time](https://x.com/i/status/2120529553135448437)
- [Supplementary same-thread detailed bo2-mac account by vibelancer, November 11, 2026 at 22:41:10 Beijing time](https://x.com/i/status/2120527258410488004)

[中文](../bo2-mac-claude-arm64-static-translation-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
