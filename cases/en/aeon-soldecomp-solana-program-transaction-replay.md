# Aeon soldecomp: a public Solana decompilation and replay workbench, now unmaintained

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-04
Stage: Related project

At 03:22:35 Beijing time on November 4, 2026, item 22 of Aaron Mars's (@aaronjmars) Aeon October report introduces soldecomp for studying deployed Solana programs and replaying real transactions locally. It is a reversing tool in an AI-agent ecosystem, not demonstrated autonomous AI recovery of arbitrary programs.

Supplementary reading of the public README is pinned to dad5fd8fc3be59f6cf67247b027bf1bb5da53493, dated October 23 at 01:33:33 Beijing time: pre-window project documentation. Its standard-library Python CLI analyzes sBPF ELF, call graphs, strings and frameworks. Ghidra emits C-like pseudocode with Solana labels; modified LiteSVM replays prior-slot account state and compares one-input mutations. Candidate Rust can be compiled and compared by bytes/score. Ghidra, Solana tools and historical RPC are additional per-command dependencies. This is neither automatic Rust-source recovery nor an exact original on-chain execution trace.

The README explicitly says released as-is, no longer maintained. Five detector classes report precision 0.83 and recall 1.0 over 13 verdicts, but the corpus is mainly synthetic controls and clean deployed programs, with only one deployed known-bug positive, historical GoonFi. field_accuracy_measurable remains false, so these are not field-effectiveness results. The repository states MIT while modified LiteSVM retains Apache-2.0. No benchmarks were executed, ELFs downloaded, accounts accessed or transactions replayed. The docs do not establish the AI model or REA used in this tool's internal analysis; related-project status is retained. The same post's papertrade map is separate.

Monthly-report candidate snapshot: 22 likes, 680 views, 7 reposts. These are whole-post engagement, not soldecomp usage.

## Sources

- [Aaron Mars's Aeon October report, item 22 on soldecomp, November 4, 2026](https://x.com/i/status/2117698975213944874)
- [Pre-window pinned README: capabilities, discontinued maintenance and synthetic-benchmark limits, October 23, 2026 Beijing time](https://github.com/aaronjmars/soldecomp/blob/dad5fd8fc3be59f6cf67247b027bf1bb5da53493/README.md)

[中文](../aeon-soldecomp-solana-program-transaction-replay.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
