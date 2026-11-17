# Windows 11 coding-tool telemetry: secondary reports of AI-assisted MissionControlAggregator analysis

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Needs verification

Candidates from 08:06 through 11:50 Beijing time on November 17, 2026 discuss Windows 11's MissionControlAggregator.dll diagnostic component. Kencouver (@mutianba) says a researcher used AI to examine recent binaries; Larry (@xqliu), at 09:39, says AI first searched for undocumented features and an agent then followed references from a tool-name list. Other candidates attribute the research to Xusheng Li and name CLICodingAgentUsage, feature ID 62580080, four CLI slots for copilot, claude, codex and agy, and five desktop slots for github, claude, codex, cursor and antigravity, with a WSL recognition path and separate traditional developer-tool entries. The goal is understanding system recognition and telemetry, not breaking these agents. Neither the AI model nor REA use is specified.

Candidates describe usage encoded as bitmaps, stored locally and included in Segments.SubCohorts ETW diagnostic events. Their statement that this record contains no code or prompts is not a guarantee about all Windows collection. The 11:45 candidate limits observations to one US-region ARM64 VM; the 11:50 candidate says the feature was off in a fresh image and could be activated by a server-side experiment. A US optional-diagnostics setting or one test cannot establish default feature activation on every PC. The 09:16 account questions actual uploads and required versus optional classification. Later advice to disable a setting, stop a service or delete diagnostics has no traffic comparison or deletion proof checked here.

Supplementary retrieval found Crackmes.one (@CrackmesOne) at 10:00:25 Beijing time on November 16 reporting tool names and ETW agent bitsets in build 26200.9974. This is pre-window background, not a replacement candidate, and does not establish that the account is Xusheng Li. Search located the reported blog address, but its text could not be read. No DLL, disassembly screenshots, original call chain or diagnostic events were examined, nor Windows hardware, packet captures or control changes tested. Status remains unverified for this secondary AI-assisted analysis account. Activation scope, uploaded fields, retention and verifiable controls remain unresolved.

November 17 sealed candidates: 08:06 post, 1 like/53 views; 09:39 post, 0 likes/210 views. Engagement does not verify system behavior.
The November 16 supplementary post had 3,087 likes, 110,211 views, 388 reposts and 111 replies when read on November 17. It is not a new-window candidate or independent verification.
November 17 at 12:56:48: copying cmd.exe and renaming it codex.exe reportedly records Codex; the component subscribes to process events rather than enumerating processes and stores data in AggregatorStorage under ProgramData. The 14:35:47 account limits testing to an ARM64 VM, build 26200.9974, enabled there but disabled in a fresh public-ISO installation; allowing optional diagnostics reportedly puts the report in DiagTrack's upload queue. The 15:18:58 account distinguishes queuing from server receipt and from scanning every installed application. None was independently rerun, and the 12:56 post's extrapolation from US diagnostic defaults does not override feature-flag limits. The three sealed sources respectively have 0 likes/69 views, 28 likes/1,448 views and 3 likes/41 views.

## Sources

- [Kencouver relays AI analysis of Windows binaries, November 17, 2026 at 08:06:53 Beijing time](https://x.com/i/status/2122481563871097208)
- [Larry relays agent reference-following from the list, November 17 at 09:39:25 Beijing time](https://x.com/i/status/2122504851016077409)
- [Secondary account questioning diagnostic bitmaps and upload classification, November 17 at 09:16:06 Beijing time](https://x.com/i/status/2122498984132698525)
- [US-region ARM64 VM and open questions, November 17 at 11:45:34 Beijing time](https://x.com/i/status/2122536597468090824)
- [Secondary account of default-off state and server-side experiments, November 17 at 11:50:35 Beijing time](https://x.com/i/status/2122537858808557839)
- [Pre-window supplement: Crackmes.one reports ETW bitsets in build 26200.9974, November 16 at 10:00:25 Beijing time](https://x.com/i/status/2122147747390468384)
- [Renaming and process-event account, November 17 at 12:56:48 Beijing time](https://x.com/i/status/2122554525169205463)
- [Build 26200.9974, public ISO and upload-queue account, November 17 at 14:35:47 Beijing time](https://x.com/i/status/2122579434934874409)
- [Account distinguishing queuing from server receipt, November 17 at 15:18:58 Beijing time](https://x.com/i/status/2122590301357531552)

[中文](../windows-missioncontrol-ai-coding-agent-telemetry-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
