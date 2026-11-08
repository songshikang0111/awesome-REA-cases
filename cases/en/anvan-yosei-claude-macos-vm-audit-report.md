# Yosei: An Van's Claude-assisted version diff, decompilation and disposable-Mac-VM audit

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-08
Stage: Needs verification

At 06:01:20 Beijing time on October 30, 2026, An Van (@anvanvan) says that before granting Yosei full control of their Mac, Claude Code agents decompiled it and ran it in a throwaway macOS VM to inspect ports, traffic, pairing and updates. The goal was deciding whether to trust another developer's software. That early post did not detail exact features or permissions. The author concluded clean, with no backdoor or phone-home, without a version, hash, decompiler output, network capture, test duration or full prompt at that time.

A new candidate at 10:23:03 Beijing time on November 8 publishes a DIY prompt: compare the newest Yosei Mac app against the installed version; verify the hash against the changelog, signature and notarization; diff the apps and decompile changed security code; run only in a disposable macOS VM, logging traffic, processes and files and probing ports; return a verdict with evidence. This describes the intended workflow, not proof that every step was performed or passed.

Supplementary same-author posts at 10:23:00 and 10:23:02 identify the version and findings. The author says they audited 0.9.15, recommends updating from 0.9.9, and credits AI assistance from Claude Opus 4.8. Their verdict is clean with findings: no backdoor, hidden data traffic or network-reachable flaw. They also flag that iPad-camera-as-Mac-webcam needs approval and could receive fake video injected by another local Mac app, which they call low risk. The default-off AI-agent setup passes an access key to Cursor/VS Code through a link, to be treated like a password. These same-day supplementary posts are not extra candidates or independent tests.

The new material supplies a version, model attribution, prompt and concrete risks, but still no actual hashes, diffs, captures, duration or replayable audit record. Not finding a network flaw does not prove the absence of all vulnerabilities, and default-off is not security certification. Earlier and later evidence remain distinct; it would now be outdated to say the author never published a full prompt. REA is not named. Only posts and the thread were read here, without running software or a VM or granting Mac control. The audit remains unverified.

October 30 candidate: 0 likes, 25 views, 0 reposts. No backdoor is the author's conclusion, not a safety guarantee by this collection.
November 8 prompt candidate: 0 likes, 4 views, 0 reposts. Supplementary version and model names retain the author's wording; audit execution is unverified.

## Sources

- [An Van's earlier Claude/macOS VM audit account, October 30, 2026](https://x.com/i/status/2115926987911078256)
- [Window candidate: version-diff, signature and VM-audit DIY prompt, November 8, 2026 at 10:23:03 Beijing time](https://x.com/i/status/2119254340062052434)
- [Supplementary author thread: 0.9.15 versus 0.9.9 audit verdict, 10:23:00 Beijing time](https://x.com/i/status/2119254330452885608)
- [Supplementary author thread: camera/key risks and Opus 4.8 attribution, 10:23:02 Beijing time](https://x.com/i/status/2119254336572424594)

[中文](../anvan-yosei-claude-macos-vm-audit-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
