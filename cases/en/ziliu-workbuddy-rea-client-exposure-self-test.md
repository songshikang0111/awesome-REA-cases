# Ziliu desktop self-test: WorkBuddy and REA reportedly expose 178 channels but find no keys

Category: Applications and clients · REA
Record date: 2026-11-13
Stage: Analysis test

At 16:26:15 Beijing time on November 13, 2026, Meng Jian (@xjtumj) reports connecting WorkBuddy to REA to analyze his own Ziliu desktop app and test whether AI could fully uncover a client he spent a year developing. He reports a 54KB analysis identifying 178 communication channels and 337 calls. A 16:26:16 follow-up reports 42,352 unknown items left by obfuscation and zero detected leaks of keys or core prompts. Another candidate at 16:28:17 repeats the report size, channels and zero-exposure claim; all belong to one self-test, not separate projects.

The author attributes the boundary to keeping core logic on the server and calls the core completely safe. This collection retains only the reported absence of detections in this static analysis. The full report, scan rules, client version, negative-detection capability and server tests are unavailable; the account does not establish that extractable secrets, authorization defects or dynamic attack paths are absent. Unknown items are not recovered features. A supplementary third post in the same thread, at 16:26:16 that day, recommends keeping prompts/keys off clients and validating local communication. These are recommendations, not implemented or verified safeguards. Neither the app nor REA was run here, and the counts were not audited.

November 13 candidate snapshots: main post 0 likes, 30 views; follow-up 0 likes, 4 views; restatement 3 likes, 312 views. All technical counts are author-reported and unaudited.

## Sources

- [Meng Jian's WorkBuddy/REA Ziliu self-test, November 13, 2026 at 16:26:15 Beijing time](https://x.com/i/status/2121157683328037250)
- [Candidate follow-up: 42,352 unknowns and no detected leaks, 16:26:16](https://x.com/i/status/2121157685714518128)
- [Candidate restatement: a year of development and a 54KB report, 16:28:17](https://x.com/i/status/2121158193971855430)
- [Supplementary defensive advice in the same thread, 16:26:16; not another candidate](https://x.com/i/status/2121157687383896415)

[中文](../ziliu-workbuddy-rea-client-exposure-self-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
