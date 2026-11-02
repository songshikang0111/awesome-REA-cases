# Lark meeting notes: WquGuru studies chunks and parallel tasks with REA, then builds a Mac version

Category: Applications and clients · REA
Record date: 2026-11-02
Stage: In progress

At 09:46:06 Beijing time on November 2, 2026, WquGuru (@wquguru) says REA helped investigate the meeting-notes implementation in the Lark desktop client, then informed a Mac rebuild planned for open-source release. The goal is progressively delivered summaries, to-dos, key decisions and chapters traceable to meeting speech, not just copying an interface.

The author reports three designs: resampling audio to 16kHz and splitting it every second, saving locally before queued uploads, deleting only after success and resuming outstanding chunks after a crash; separate generation and timeout handling for each type of note so finished results appear first; and fishbone diagrams whose branches link back to original sentences and count supporting citations. These are the author's analysis and reconstruction claims. No target version, located functions, source or crash-recovery tests are provided. A queue design does not guarantee that recordings can never be lost, and citation counts do not establish semantic accuracy.

Supplementary reading of the same author's thread finds an 11:09:17 reply saying release will follow a complete test pass, and an 11:44:21 reply naming the model as 'ds v4.1 flash 1017'. These are same-day supporting sources, not new independent candidates. Free models, no self-hosting and fully open source remain promises. The model provider, limits and data destination are unspecified; this does not establish offline operation or meeting privacy. Other platforms are reader suggestions, not implemented support. No public repository was obtained, no tool installed or run, no Lark connection made and no meeting data accessed.

Sealed candidate snapshot: 93 likes, 7,425 views and 7 reposts. Engagement does not establish completed implementation tests.
16kHz and one-second chunks are the author's analysis; open-source availability, free models and full test results remain unconfirmed.

## Sources

- [WquGuru's Lark meeting-notes investigation and Mac-rebuild report, November 2, 2026](https://x.com/i/status/2117070715803640272)
- [Same-day author follow-up: release after full testing, 11:09:17 Beijing time](https://x.com/i/status/2117091650644418813)
- [Same-day author model identification: ds v4.1 flash 1017, 11:44:21 Beijing time](https://x.com/i/status/2117100475413877105)

[中文](../wquguru-lark-rea-mac-meeting-notes-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
