# BLA versus REA: public decoy and resource-budget tests, not a guarantee against reversing

Category: Applications and clients · REA
Record date: 2026-11-01
Stage: Analysis test

At 15:45:00 Beijing time on October 29, 2026, 0xMarioNawfal (@RoundtableSpace) presents BLA (Blind LLM Agents), saying it inserts decoys and resource-consuming structures into release artifacts so REA fails or exceeds budgets while user behavior is preserved. Supplementary npm metadata maps bla-agents to qybaihe/bla. This is a related defensive project for one's own software, not reconstruction of a third-party app.

The repository README and empirical-rea-validation report were read at pinned commit e5a566a3f544f69ef8bbe153e721f1555901578a. The report is dated October 27, 2026, 09:56 Asia/Shanghai, using Node v24.22.1 and tshark 4.4.19, before the candidate and supplementary only. The project compares samples before and after hardening through real REA analysis paths, reporting Go buildinfo beyond 1MiB, BEAM beyond 64 chunks, ASAR headers beyond 16MiB, plus JavaScript semantic budgets, model-metadata nesting, SQLite trap columns and WASM representation limits.

The report retains counterexamples and method boundaries: hardened EVM remains status=ok and only approaches the 4MiB input cap; Flutter uses a replica of private projection logic and remains ok; PTX text does not hit a budget. The ASAR error explains that settings can raise the default cap, so default rejection is not permanent unanalyzability. Ghidra/Hopper, Frida, LLDB/GDB, Rizin, JADX and other native/dynamic paths were not empirically tested in that environment. Firmware and several GPU formats are skipped.

The README explicitly labels the 14-target approximately 612.5× token and 292.2× cost figures as internal estimates, distinct from real analyzer errors. Its 14/14 runtime-equivalence result is a project sample check, not a guarantee about arbitrary software semantics, performance or maintainability. Repository documentation stages v1.4.0, while queried npm latest remains 1.1.0, published October 25; they are not treated as the same published revision.

This does not independently prove a cloud LLM agent spent its budget, followed decoys or failed end-to-end reconstruction. The pinned report also did not provide a REA revision this collection could confirm. No BLA installation, target-code execution or test rerun occurred here; only public project reports were statically read. Included as a counter-REA analysis test with public code and limitations, not a protection guarantee.

Earlier candidate snapshot: 10 likes, 10,035 views, 1 repost. New candidate: 1 like, 457 views, 0 reposts; the older snapshot is preserved.
Project measurements cover bounded sample analyzer paths. Token/cost multipliers are estimates, not independently rerun.
Earlier supplementary evidence: October 27 report; pinned repository commit time 2026-10-28T18:09:36Z, not newly published in this window.
A Japanese report at 14:48:02 on November 1 adds version details: GitHub 1.5.2 adds a decoy DEX with external method calls to unsigned APKs, while empirical JADX testing remains planned; 1.5.1 reportedly fixes breakage of Bun standalone executables, and npm is still reported as 1.1.0. These are secondary release descriptions, without reading the pinned implementation or rerunning validation for those revisions. The older 1.4.0 material is not empirical proof for 1.5.2.

## Sources

- [0xMarioNawfal introduces BLA and counter-REA results, October 29, 2026](https://x.com/i/status/2115711483049083166)
- [Supplementary: pinned BLA README separating measured paths, estimates and untested capabilities](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [Supplementary: October 27 project before/after REA-analyzer validation report at a pinned commit](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [Supplementary: npm metadata and October 25 publication record](https://registry.npmjs.org/bla-agents)
- [New: secondary release account of 1.5.2 APK decoy DEX and 1.5.1 Bun repair, November 1, 2026](https://x.com/i/status/2116784310317732268)

[中文](../bla-counter-rea-budget-decoy-validation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
