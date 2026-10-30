# winutil and Windows tweaks: gIoomy's Opus-audit account retains contradictory counts

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-30
Stage: Needs verification

At 06:14:50 Beijing time on October 30, 2026, gIoomy (@0xgIoomy) says Claude Code with Opus 5.5 investigated the open-source Windows optimizer winutil before auditing their PC. The model reportedly read all 39 tweaks without changes, skipped disabling BitLocker in the essential section and noticed that undo restores Windows defaults rather than the user's previous values. It therefore backed up actual values, created a restore point and selected seven tweaks for winutil to apply. This describes understanding an open-source tool's behavior for local maintenance, not established decompilation of a proprietary optimizer. REA is not mentioned.

The opening claims startup apps fell from 24 to 11 and 18GB of temporary files became zero. The read-only inventory gives 24 startup apps, 18GB and 87 services; the final post-reboot figures instead give 17 to four startup apps, 142 to 64 services and 18GB to zero. These inconsistent scopes are preserved rather than turned into a unified reduction, speedup or safety result. The claim that everything is reversible has no backup inventory, recovery rehearsal, Windows version or performance measurement. Calling seven tweaks safe is the author's judgment, not a guarantee here.

Original attribution and full text were checked, without an exact winutil commit, the selected seven tweaks or test output. No optimizer was run, BitLocker changed, temporary files deleted or services modified here. Retained as an unverified workflow report.

Candidate snapshot: 5 likes, 213 views, 0 reposts.
Startup apps 24→11 versus 17→4 and services 87 versus 142→64 are inconsistent. The 39 reviews, seven selections and 18GB are author reports; rollback is unverified.

## Sources

- [Candidate: gIoomy's account of Opus reviewing winutil and applying PC tweaks, October 30, 2026](https://x.com/i/status/2115930385494528262)

[中文](../gloomy-winutil-opus-readonly-tweak-audit.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
