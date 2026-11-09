# BLA versus REA: public decoy and resource-budget tests, not a guarantee against reversing

Category: Applications and clients · REA
Record date: 2026-11-10
Stage: Analysis test

At 15:45:00 Beijing time on October 29, 2026, 0xMarioNawfal (@RoundtableSpace) introduces BLA (Blind LLM Agents), claiming decoys and resource-consuming structures in release artifacts make REA fail or exceed budgets while preserving user behavior. npm metadata maps bla-agents to qybaihe/bla. This defends one's own software, not reconstructing a third-party application.

Earlier supplementary reading covers README and empirical-rea-validation at e5a566a3f544f69ef8bbe153e721f1555901578a. The report is dated October 27, 09:56 Asia/Shanghai, with Node v24.22.1 and tshark 4.4.19; the commit is 2026-10-28T18:09:36Z. Samples invoke real REA paths and report Go buildinfo over 1MiB, BEAM over 64 chunks, ASAR headers over 16MiB, JS semantic budgets, nested model metadata, SQLite trap columns and WASM representation limits. EVM remains ok near the 4MiB cap; Flutter replicates private projection logic and remains ok; PTX does not hit a budget. ASAR's cap can be raised, so rejection is not permanent unanalyzability. Native/dynamic Ghidra/Hopper, Frida, LLDB/GDB, Rizin and JADX paths are untested; firmware and some GPU formats are skipped. Roughly 612.5 times the tokens and 292.2 times the cost across 14 targets are internal estimates, not paid consumption. The 14/14 runtime-equivalence sample check does not guarantee arbitrary semantics, performance or maintainability.

Older docs stage v1.4.0, distinct from then-current npm 1.1.0 published October 25. A November 1, 14:48:02 Japanese account describes GitHub 1.5.2 adding external-method-call decoy DEX to unsigned APKs, with JADX tests still planned, and 1.5.1 fixing broken Bun standalone executables; it still reports npm 1.1.0. Pinned implementations were not read or retested. At 10:40:42 on November 7, KitPloit (@KitPloit) introduces 3.0.0 protection for binaries, ASAR, JS, WASM, Python and model files; attribution was checked. Earlier supplementary npm reading confirms 3.0.0 at 2026-11-06T09:16:07.184Z, repository qybaihe/bla and then-latest 3.0.1. Registration is pre-window background, not effectiveness evidence. The 3.0.0 code/tests were not reviewed; the old pinned report does not validate every newer format.

A new November 10, 01:55:31 candidate cites i10x saying an Electron project sample grows from 607 B to 16.9 MiB and fake credentials may trigger app-store review or security scanners. It advises testing hardened builds and keeping real secrets server-side. A 03:15:20 candidate says a 607-byte file grows to 17MB and REA errors, similarly across nine formats, while a screenshot-driven agent bypasses this path. Units and rounding are preserved rather than combined into an invented multiplier. The i10x article, new samples, agent logs and screenshot-route tests were not obtained, so size, nine-format coverage and screenshot limitations remain relayed claims, not new measurements here. They add distribution/review costs and distinguish analyzer and GUI paths, not proof that all agents exhaust budgets or every screenshot agent succeeds.

This is not independent proof of cloud-LLM decoy pursuit, budget exhaustion or failed complete reversing. The old report's exact REA revision is unconfirmed. Only public text and metadata were read; no installation, target execution or reruns occurred here. Status remains analysis-test without a protection guarantee.

Earlier candidate: 10 likes, 10,035 views, 1 repost; November 1: 1 like, 457 views, 0 reposts. Older snapshots retained.
Bounded sample analyzer paths; token/cost multipliers are estimates, not independently rerun.
The October 27 report does not validate 3.0.0. November 7 candidate: 2 likes, 663 views, 1 repost.
November 10 sealed additions respectively: 0 likes/15 views/0 reposts and 0 likes/7 views/0 reposts. Size and screenshot routes were not retested.

## Sources

- [0xMarioNawfal introduces BLA and counter-REA results, October 29, 2026](https://x.com/i/status/2115711483049083166)
- [Supplementary pinned BLA README separating measured paths, estimates and untested capabilities](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [Supplementary October 27 project before/after analyzer validation at a pinned commit](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [Supplementary npm registration, reread November 7 for the 3.0.0 date and repository](https://registry.npmjs.org/bla-agents)
- [Secondary 1.5.2 APK decoy DEX and 1.5.1 Bun repair account, November 1, 2026](https://x.com/i/status/2116784310317732268)
- [KitPloit's bla-agents-3.0.0 introduction, November 7 at 10:40:42 Beijing time](https://x.com/i/status/2118896395687981497)
- [New account: 607 B to 16.9 MiB and fake-credential review risks, November 10 at 01:55:31 Beijing time](https://x.com/i/status/2119851392353345740)
- [New account: 17MB errors and screenshot-driven agent limits, November 10 at 03:15:20 Beijing time](https://x.com/i/status/2119871480838148149)

[中文](../bla-counter-rea-budget-decoy-validation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
