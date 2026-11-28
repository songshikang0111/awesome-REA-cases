# MiniMax's VM-protection logic recovery: a project evaluation on 100 internal samples

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-28
Stage: Analysis test

A brief candidate at 21:45:00 Beijing time on November 28, 2026 says MiniMax's strongest internal model automatically recovered logic in over 90% of virtualized-protection samples. At 21:47:11, Hard Signal (@cccc2024cccc) provides a more specific account. The targets are protections such as VMProtect and Themida that translate instructions into private bytecode executed by a custom virtual machine, not hardware-VM escape. This is separate from the same evaluation's Rust decompiler-core replacement.

The later account describes 100 difficult internal samples, a 70% autonomous single-attempt recovery rate and 94% aggregate recovery with verifier feedback and eight samples. It says the VMProtect 3.x/Themida group exceeds 90%. The reported wording is preserved: subgroup sizes, per-task success criteria and sampling aggregation are absent. Ninety-four percent is not presented as a single-attempt rate, nor is a subgroup's over-90% result extended to every tool and version.

The post acknowledges markedly lower initial success with nested virtualization or strong anti-debugging, and oversized traces exhausting context and causing ineffective debugging loops. The model is unreleased and relies on custom scaffolding, not proof of equivalent capabilities in currently available models. Moving high-value logic server-side, hardware trusted execution and dynamic protection are relayed recommendations, not established effective defenses.

Retrieval confirmed the later post's attribution and full wording. Supplementary reading then covered MiniMax's original website evaluation dated November 28, 2026, confirming the project's 100 samples, 70.00% single-attempt rate, 94.00% aggregate with eight samples and over 90.00% for the VMProtect 3.x/Themida group. The report describes static localization followed by dynamic observation, symbolic reasoning into readable C/C++, and input/output iteration until the verifier passes. This summarizes the research method without bypass procedures. Tens of minutes is a company-level description without per-task timings, not a result assigned to every sample. No publication time is given; the report is supplementary evidence, not a new strict-window candidate.

The dataset, verifier, revision configuration and runtime logs were not obtained, preventing independent checks of success criteria, authorization, sample independence and applicability to commercial software. The company says all code, artifacts and logs were destroyed after isolated evaluation, never distributed or commercialized, and public capabilities may be restricted. Those statements are not independently audited. This collection installed no model, executed no protected sample and reran no experiment. Status remains analysis-test with attribution to internal self-evaluation; REA is unmentioned.

Sealed snapshots: first post 2 likes, 157 views, 0 reposts, 0 replies; later post 0 likes, 47 views, 0 reposts, 0 replies. An internal set, not a public leaderboard; no independent reproduction here.

## Sources

- [Overview of MiniMax's internal protection-logic recovery, November 28, 2026 at 21:45:00 Beijing time](https://x.com/i/status/2126673716956529120)
- [Supplementary company report: 100 samples, single/multiple-attempt metrics and limits, dated November 28, 2026 with no time](https://www.minimax.cn/blog/minimax-internal-model-reverse-engineering-evaluation)

[中文](../minimax-internal-vmprotect-themida-devirtualization-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
