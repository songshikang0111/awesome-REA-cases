# A CleanMyMac/CCleaner-style cleaner: an Opus screenshot rebuild and deletion-safety account

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-30
Stage: Needs verification

At 02:16:22 and 02:48:44 Beijing time on October 30, 2026, two candidates describe the same CCleaner/CleanMyMac-style cleaner workflow. Claude Code with Opus 5.5 receives a long prompt and CleanMyMac screenshots, proposes nine UI concepts and uses eight parallel agents for a scanner, disk map, AI assistant, startup items and installers. The stack is Electron/React, with GitHub Actions reportedly building a Mac dmg and Windows exe. The described evidence is screenshot- and behavior-led reconstruction, not established binary analysis of either product. REA appears only in the appended course promotion, so its use in this project is unconfirmed.

The author says a separate safety agent caught a DOCUME~1 short-path issue that could send all of Documents to the Recycle Bin and an icon loader that could leak a Windows password hash, reportedly fixed. A startup toggle first falsely reported that Windows refused a change; PowerShell allegedly lost the exit code after elevation, so registry checking replaced it. The later post adds a policy of deleting caches directly while sending user-created material to Trash first. These are reported reviews and policies, not safety guarantees here. Built-in Claude/ChatGPT reportedly sees only names and sizes, not contents; names can still contain sensitive information, so this does not establish complete privacy.

The author claims one afternoon, no manually written code and 14.6GB freed on the first click; the other post compares it with $40/year cleaners. Repository, releases, platform tests, deletion lists, space accounting and pricing were not checked. A draggable physics-bubble disk map and smoky WebGL background are described features, not proof of correct cleanup. Distinguished from existing native-Mac cleaner prototypes. This collection did not install software, delete files or reproduce safety tests. Status remains unverified.

Candidate snapshots: 51 likes/2,676 views/5 reposts and 24 likes/1,232 views/1 repost.
One afternoon, 14.6GB, $40/year and safety fixes are author accounts, not independent measurements or audits.

## Sources

- [Candidate reports screenshot reconstruction, deletion-path review and startup-item fixes, October 30, 2026](https://x.com/i/status/2115870373300326503)
- [Same-window follow-up: cache/user-file policy and 14.6GB claim, October 30, 2026](https://x.com/i/status/2115878519901229474)

[中文](../opus-cleanmymac-ccleaner-electron-rebuild-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
