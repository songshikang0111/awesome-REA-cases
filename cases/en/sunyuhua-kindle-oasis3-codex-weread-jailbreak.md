# Kindle Oasis 3: Codex helps debug a jailbreak; the author opens a WeRead book

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-02
Stage: Needs verification

At 17:55:05 Beijing time on November 2, 2026, monkey-king.sun (@sunyuhua0205) reports connecting a Kindle to a Mac to use WeRead. Supplementary lookup retrieves the full ending. The device is a tenth-generation 32GB Kindle Oasis 3 on firmware 5.17.1. The final setup uses Nosebleed with a locally staged v2.5.0 jailbreak installer, KOReader 2026.07.1's kindlehf package and finlater/weread.koplugin v1.6.0. This is AI assistance with existing community jailbreak and reading interoperability, not Codex discovering a new vulnerability or writing a reader.

The author reports only about 60MiB free because of update-blocking placeholder files. Codex identified USB details, checked community guidance and made backups. The first SpiderCat ebook would not open: its hash matched, but a .bad_file cache marker existed. After clearing and retrying, execution stalled for an hour. A log with uid=0 euid=0 established prior privilege elevation, not completed installation. They switched to Nosebleed, staged the roughly 5MB main installer locally without changing the original project's binaries or main script, and captured output. The device then rebooted automatically and produced a 'You are jailbroken!' completion file. The author explicitly leaves the original stall unexplained, rather than claiming a proven network failure.

The installation log still contains a system-patch component anomaly, but the author subsequently reports launching KOReader, completing WeRead QR login and opening a book. Reader and plugin copying/content checks covered 1,125 files; deleting old placeholders restored about 26.6GiB free space. Codex handled computer-side checks, downloads, backups, script preparation and logs. The human handled Kindle clicks, reboots, Wi-Fi and phone authorization; the key did not need to be shared with Codex.

Versions, space, file counts and reading results are author reports without raw logs, long-term stability checks or independent reproduction here. Other devices and firmware require fresh compatibility checks. REA is unspecified. No jailbreak payload was downloaded, script executed, account accessed or device operated.

Candidate snapshot: 0 likes, 48 views, 0 reposts. Full original text retrieved; attached image uninspected.
uid=0 does not establish completed installation. The completion marker and actual book opening are distinct author-reported validation stages.
Reuses community tools, not an AI-original vulnerability. The first stall's cause and patch anomaly remain visible.

## Sources

- [monkey-king.sun's full Kindle/Codex debugging and book-opening account, November 2, 2026](https://x.com/i/status/2117193771062554902)

[中文](../sunyuhua-kindle-oasis3-codex-weread-jailbreak.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
