# Lark meeting notes: WquGuru studies chunks and parallel tasks with REA, then builds a Mac version

Category: Applications and clients · REA
Record date: 2026-11-03
Stage: In progress

At 09:46:06 Beijing time on November 2, 2026, WquGuru (@wquguru) says REA helped investigate the meeting-notes implementation in the Lark desktop client, then informed a Mac rebuild planned for open-source release. The goal is progressively delivered summaries, to-dos, key decisions and chapters traceable to meeting speech, not just copying an interface.

The author reports three designs: resampling audio to 16kHz and splitting it every second, saving locally before queued uploads, deleting only after success and resuming outstanding chunks after a crash; separate generation and timeout handling for each type of note so finished results appear first; and fishbone diagrams whose branches link back to original sentences and count supporting citations. These are the author's analysis and reconstruction claims. No target version, located functions, source or crash-recovery tests are provided. A queue design does not guarantee that recordings can never be lost, and citation counts do not establish semantic accuracy.

Supplementary reading of the November 2 author thread finds an 11:09:17 reply saying release will follow a complete test pass, and an 11:44:21 reply naming the model as 'ds v4.1 flash 1017'. These are earlier supporting sources, not new candidates in this window. At 19:27:14 on November 3 the author claims the client is now fully open source, models are free and commercial modification is allowed, supplying GitHub, website and model short links. This is author-reported release progress beyond the earlier plan, not source or license inspection by this collection.

The update lists Tencent Meeting, Lark, DingTalk, WeCom, Zoom, Google Meet, Microsoft Teams, Webex, X Spaces, Discord, Telegram, Clubhouse and YouTube, Twitch and Bilibili livestreams as input scenarios. Without a compatibility matrix or per-platform tests, system-audio capture, dedicated connectors and official integration cannot be distinguished. They are not separate projects. The model provider, limits, data destination and full test results are unspecified. 'More powerful', 'free' and unrestricted commercial modification are author claims, not equivalence acceptance, total-cost findings or legal certification. Inspectable public repository contents were not obtained; no tool was installed or run, no Lark connection made and no meeting data accessed. Offline operation, meeting privacy and zero recording loss are not guaranteed.

November 2 sealed snapshot: 93 likes, 7,425 views, 7 reposts. November 3 candidate: 13 likes, 894 views, 2 reposts. Engagement does not establish completed tests.
16kHz and one-second chunks are the author's analysis. Current open-source, free-model, licensing and platform-scope statements are author claims without source inspection or runtime tests.

## Sources

- [WquGuru's Lark meeting-notes investigation and Mac-rebuild report, November 2, 2026](https://x.com/i/status/2117070715803640272)
- [Same-day author follow-up: release after full testing, 11:09:17 Beijing time](https://x.com/i/status/2117091650644418813)
- [Same-day author model identification: ds v4.1 flash 1017, 11:44:21 Beijing time](https://x.com/i/status/2117100475413877105)
- [Window author update: claimed open-source release, free models and multiple input platforms, November 3, 2026, 19:27:14 Beijing time](https://x.com/i/status/2117579351583830022)

[中文](../wquguru-lark-rea-mac-meeting-notes-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
