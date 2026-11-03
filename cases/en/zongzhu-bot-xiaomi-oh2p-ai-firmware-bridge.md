# Xiaomi Speaker Pro meets Grok Bot: reported Claude/Codex patching and dual-wake-word bridging

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-03
Stage: In progress

At 15:21 Beijing time on November 3, 2026, AI少年 (@aehyok) introduces Drunk's (@Liu_zhongxisn) zongzhu-bot speaker tutorial: Xiaomi Smart Speaker Pro OH2P, firmware 1.62.2 and an Apple-silicon Mac. The original XiaoAI wake phrase still plays music; another phrase routes to a personal Grok Bot and speaks its response. The aim is retaining device interaction while adding a personal agent, not running the Grok model locally on the speaker.

The post says prompts guide Claude Code or Codex through configuring the feat/gateway backend, generating a matching-firmware patch image, backup and Client compilation, with the Mac bridge and backend relaying requests. Daily use is over Wi-Fi and requires both backend and bridge to stay running on the Mac. Retaining firmware means patching the original system, not leaving the device entirely unchanged; the post says Xiaomi auto-updates are disabled. Only interoperability and backup boundaries are summarized, not flashing instructions.

Three reportedly merged fixes are listed: bridge misclassification of XiaoAI events as interruptions stopped music after two seconds; duplicate wake events caused long responses to time out; standby disconnection produced only a short acknowledgement, addressed by reconnecting on wake. Acceptance must therefore hear an actual complete answer, not merely a wake acknowledgement.

LX06 compatibility on the same firmware is attributed to the original tutorial; other models/versions were not run. Windows feasibility is the reposter's guess, not supported-platform evidence. The 245 stars are a post claim, not checked against a repository snapshot. No confirmed repository, patch diff, firmware verification or independent run record was obtained, nor a detailed human/AI division of reversing and patching work. Autonomous model completion is not established. REA is unspecified. No firmware was downloaded, device flashed or bot connected here.

Candidate snapshot: 2 likes, 253 views, 0 reposts. The 245 stars are a secondary claim without repository verification, not engagement measured here.

## Sources

- [AI少年 recounts Drunk's Xiaomi speaker/Grok Bot tutorial and fixes, November 3, 2026](https://x.com/i/status/2117517451038720170)

[中文](../zongzhu-bot-xiaomi-oh2p-ai-firmware-bridge.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
