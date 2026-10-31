# Agent-PAL: a benchmark report from DOS PAL engine investigation to full-game completion

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-01
Stage: Analysis test

At 02:10:55 Beijing time on November 1, 2026, Jianming Liu (@jianmliu) introduces his Agent-PAL framework, reporting two weeks comparing models playing the 1995 DOS Chinese Paladin game. Its pure mode is described as L0 with no scaffolding, walkthrough or pathfinding API, requiring models to investigate the engine and write even battle scripts from scratch to reach the ending across 11 chapters. AI reverse engineering is therefore a prerequisite for game control, not merely answering questions.

He reports three wins in three runs for Gemini 4 Argon, GPT-6.1-Sol and Claude Opus 5.5, averaging 2.6 hours. The DeepSeek V4 Pro/V4.1-Flash, GLM-5.3, Kimi K3 and MiniMax M3 group reportedly spends 51.30 hours, 20,192 tool calls and 1.983 billion tokens, fails to finish despite one human hint, and DeepSeek exhausts its monthly allowance at turn 428. Figures, grouping/aggregation and the open-source claim belong to the post; no turn-level code, seeds, billing or acceptance logs were obtained for verification.

The author's explanation in terms of training-induced mental friction is not independently established by this evidence, nor a general ranking by model nationality. No game was run, framework installed or completion retested. REA is not named; retained as an author-reported benchmark.

Candidate snapshot: 0 likes, 43 views; consumption and completion are author reports.

## Sources

- [Jianming Liu's Agent-PAL benchmark account, November 1, 2026](https://x.com/i/status/2116593778798502051)

[中文](../agent-pal-dos-pal-ai-engine-benchmark-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
