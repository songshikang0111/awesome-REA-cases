# BLA versus REA: public decoy and resource-budget tests, not a guarantee against reversing

Category: Applications and clients · REA
Record date: 2026-11-07
Stage: Analysis test

At 15:45:00 Beijing time on October 29, 2026, 0xMarioNawfal (@RoundtableSpace) presents BLA (Blind LLM Agents), claiming decoys and resource-consuming structures in release artifacts make REA fail or exceed budgets while preserving user behavior. npm metadata maps bla-agents to qybaihe/bla. This protects one's own software rather than reconstructing a third-party app.

Earlier supplementary reading covered README and empirical-rea-validation at e5a566a3f544f69ef8bbe153e721f1555901578a. The report is dated October 27 at 09:56 Asia/Shanghai, using Node v24.22.1 and tshark 4.4.19; the pinned commit is timestamped 2026-10-28T18:09:36Z. Both are older evidence. Before/after samples call real REA paths, reporting Go buildinfo over 1MiB, BEAM over 64 chunks, ASAR headers over 16MiB, and JavaScript semantic, model-metadata nesting, SQLite trap-column and WASM representation budgets.

Counterexamples include EVM still status=ok near the 4MiB input cap; Flutter using a replica of private projection logic and remaining ok; and PTX not triggering a budget. ASAR's default cap can be raised, so rejection is not permanent unanalyzability. Ghidra/Hopper, Frida, LLDB/GDB, Rizin, JADX and other native/dynamic paths were not tested in that environment; firmware and some GPU formats were skipped. Approximately 612.5 times the tokens and 292.2 times the cost across 14 targets are internal estimates, not paid consumption. The 14/14 runtime-equivalence sample check does not guarantee arbitrary semantics, performance or maintainability.

Older documentation staged v1.4.0 while npm latest was then 1.1.0, published October 25; those are not the same revision. A Japanese account at 14:48:02 on November 1 describes GitHub 1.5.2 adding a decoy DEX with external method calls to unsigned APKs, with empirical JADX tests still planned, and 1.5.1 fixing broken Bun standalone executables; it still reported npm 1.1.0. Those pinned implementations were not read or retested, and the older evidence does not validate newer versions.

At 10:40:42 on November 7, KitPloit (@KitPloit) introduces bla-agents-3.0.0, claiming decoy metadata, budget exhaustion and runtime-equivalent shields for binaries, Electron ASAR, JS, WASM, Python and model files. Retrieval confirms attribution. Subsequent read-only npm metadata confirms 3.0.0 was published at 2026-11-06T09:16:07.184Z, with repository qybaihe/bla; latest was 3.0.1 when read. The registration predates this window and is supplementary, not a new candidate; a latest tag does not prove protection. No 3.0.0 implementation, tests or full changelog was reviewed. Older pinned tests cannot establish effectiveness across all formats in that release.

This is not independent proof of a cloud LLM exhausting its budget, following decoys or failing full reconstruction. The old report's exact REA revision is also unconfirmed. This collection read public text and metadata only, without installation, target execution or reruns. Status remains analysis-test, without a protection guarantee.

Earlier candidate: 10 likes, 10,035 views, 1 repost. November 1 candidate: 1 like, 457 views, 0 reposts; older snapshots are retained.
Project measurements cover bounded sample analyzer paths. Token/cost multipliers are estimates, not independently rerun.
The October 27 report and old pinned commit do not validate 3.0.0. November 7 sealed candidate: 2 likes, 663 views, 1 repost.

## Sources

- [0xMarioNawfal introduces BLA and counter-REA results, October 29, 2026](https://x.com/i/status/2115711483049083166)
- [Supplementary: pinned BLA README separating measured paths, estimates and untested capabilities](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [Supplementary: October 27 project before/after REA-analyzer validation report at a pinned commit](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [Supplementary npm registration, reread November 7 for the 3.0.0 date and repository](https://registry.npmjs.org/bla-agents)
- [Secondary release account of 1.5.2 APK decoy DEX and 1.5.1 Bun repair, November 1, 2026](https://x.com/i/status/2116784310317732268)
- [KitPloit's bla-agents-3.0.0 introduction, November 7, 2026 at 10:40:42 Beijing time](https://x.com/i/status/2118896395687981497)

[中文](../bla-counter-rea-budget-decoy-validation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
