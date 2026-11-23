# Reverify: deterministically check an agent's binary claims; 97% is not every model's error rate

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-23
Stage: Analysis test

At 18:42:13 Beijing time on November 23, 2026, a candidate introduces 2akouwu/reverify and its Propose→Verify→Evidence workflow for reducing hallucinated fields, offsets and function behavior, alongside persistent context. The public README and BENCHMARK.md were read at commit f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923, dated 2026-09-07T10:12:05Z, before the window. CLI/MCP claims are checked against actual artifacts through parsing, disassembly, matching or emulation, returning VERIFIED, REFUTED or INCONCLUSIVE with evidence. Source-equivalence comparison and cross-session ledger/rollover are also documented project features.

The candidate's 97% claim requires narrowing. BENCHMARK describes blindly applying the textbook push rbp; mov rbp,rsp prologue prior to 71 Windows 11 x86/x64 files. It mismatches 69; zero incorrect claims are accepted, and restating observed instructions after one feedback round reaches 71/71. This is not 71 independent queries to a live model or a general AI error rate. The reference record is dated September 4, 2026, using reverify 0.10.0, Python 3.14, capstone and lief. Zero false acceptances still has a reported 95% upper bound of 5.1%.

Documentation also reports three-platform CI and an external aarch64 run, while acknowledging limits including continued x86_64 slice selection for macOS universal files. Only documentation was read here, not raw per-file records, CI artifacts or external replication evidence. No binary, emulator or model was executed. Deterministic verification checks supplied claims within engine coverage; it is not proof of complete recovered source or semantic equivalence. REA is unmentioned.

Candidate: 6 likes, 453 views, 0 reposts, 4 replies. Its 1,351-star figure is a post snapshot, not a measurement performed here.
69/71, zero false acceptances and 71/71 describe the project's prologue-prior benchmark, not general accuracy.

## Sources

- [Candidate introduces Reverify, November 23, 2026 at 18:42 Beijing time](https://x.com/i/status/2124815780789534878)
- [Supplementary README pinned to a 2026-09-07T10:12:05Z commit](https://github.com/2akouwu/reverify/blob/f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923/README.md)
- [Supplementary benchmark methods and limitations at the same commit](https://github.com/2akouwu/reverify/blob/f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923/BENCHMARK.md)

[中文](../reverify-binary-claims-deterministic-verifier.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
