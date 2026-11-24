# REA analysis: a binary prompt-injection test idea

Category: Algorithms and feature recovery · REA use unconfirmed
Record date: 2026-11-24
Stage: Needs verification

riyoway proposes placing AI-directed instructions in target strings, resources or dead code to observe whether LLM reverse-engineering tools such as REA treat them as instructions and contaminate analysis. The aim is to assess indirect prompt-injection boundaries in AI reverse-engineering workflows. Initially the author only considered an experiment, with no sample, test or success evidence. This collection did not create or execute an injected target, and the proposal is not presented as an effective defense.

Later test (author report): the author used REA 6.5.0's JavaScript analyzer on a self-made toy Electron app without connecting an agent and searched reports for nine harmless markers. Six appeared in different report sections. Comments and package.json description did not appear; some strings, object keys, IPC names, URLs and filenames did. Slices containing only summary/statistics/limitations and window settings lacked the markers, while the window slice still showed nodeIntegration enabled and contextIsolation disabled. The author consequently recommends checking numbers and flags first and treating slices with names or URLs as target text. This shows only which sample text enters static-analysis output, not that a model follows instructions, and cannot be generalized to other commands or apps.

At 21:00:53 Beijing time on November 24, 2026, AI in Practice (@ai_kra_name) separately proposes double-encrypting executable strings and adding prompt-injection text to mislead AI reversing, alongside checking a key available only on the developer's machine and comparing its SHA-256 hash. Supplementary retrieval confirms attribution. The content is a third-person summary without identifying the original proposer, target program or implementation; it is not a new riyoway experiment. No sample, key-management design, tested model, comparison or bypass result is supplied. Model obedience, encryption preventing analysis and a reliable local-key defense are not established. This collection only records the specific combined idea without creating or executing it, maintaining the distinction between static text reaching a report and a model being induced to obey it.

Posted: 2026-10-12T23:42:14+08:00 (Beijing time)
Engagement snapshot (2026-10-13): 1 like | 14 views | 0 reposts
REA 6.5.0; author's self-made toy Electron app; no agent connected and no test of model obedience to embedded text.
At 20:30 on October 15, another user proposed embedding text in their own software requiring a model to repeat interjections many times as interference against AI reverse engineering. This adds only a concrete idea, not new results from the earlier experiment's author, and establishes neither agent obedience nor an effective defense. Candidate snapshot: 36 likes and 1,450 views, recorded October 16.
November 24 sealed candidate: 0 likes, 5 views, 0 reposts, 0 replies. Neither model obedience nor encryption effectiveness was tested.

## Sources

- [Author report from this review](https://x.com/i/status/2109670989319868863)
- [Author's REA 6.5.0 toy-app static-analysis test (model obedience untested)](https://x.com/i/status/2110441399279604113)
- [Another user's embedded-prompt interference idea (untested)](https://x.com/i/status/2110709861042503706)
- [AI in Practice relays double string encryption, prompt injection and a local-key hash idea, November 24, 2026 at 21:00:53 Beijing time](https://x.com/i/status/2125213061610885475)

[中文](../rea-binary-injection-test-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
