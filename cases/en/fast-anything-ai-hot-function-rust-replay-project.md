# fast-anything: record hot-function behavior and rebuild only the slow parts in Rust

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-22
Stage: Related project

At 17:38:17 Beijing time on November 22, 2026, mingzi206 (@mingzi206) introduces EL4CTEO's fast-anything. It aims to retain most existing application code while Claude Code or Codex ports time-consuming functions to Rust. Included as a broader AI-assisted behavior-reconstruction tool, not evidence of closed-source binary decompilation or use of REA. The slowest 5% is positioning, not a measured fraction for every application.

Supplementary reading pins the README to ebc04b09aabad2b759d7791d4d0c997e0a9fbd01, committed at 19:59:12 Beijing time on November 22, after the candidate. This is later project documentation, not the version available when the post appeared. The workflow profiles time and portability, records up to 500 real calls, generates a one-function Rust crate and TASK.md, builds and replays calls. The original supplies reference answers for additional edge cases and shrunken inputs. Docs report catching a bytes-versus-characters mistake on 148 of 500 calls, a floating-point tolerance of 1e-9, matching errors and refusal to enable ports slower per call. Finite input checks with tolerances are not formal equivalence for every input. Recording runs the original program and does not establish zero side effects or risk.

Project-reported Python fuzzy deduplication of 700 names on an i5-10500 running Windows 11 goes from 4.91 seconds to 42 milliseconds, labeled 116×. The same table reports TypeScript 20×, PHP 55× and Go 21×. C/C++ instead use a four-core GitHub Actions Linux runner, not the same environment. A Java example reports an 11× function gain but 3× for the app, retaining the startup-cost distinction. Docs prefer moving outer loops to reduce cross-language calls, and describe disabling or removing inserted blocks. Scope is top-level deterministic functions or corresponding static methods taking plain data, not all stateful, I/O or device behavior. Only documentation was read; nothing was installed, executed, compiled or benchmarked here. Language support and passing tests remain project reports.

Sealed snapshot: 32 likes, 2,294 views, 3 reposts, 5 replies. Engagement and benchmark headlines do not replace independent validation.

## Sources

- [mingzi206 introduces fast-anything, November 22, 2026 at 17:38:17 Beijing time](https://x.com/i/status/2124437302068011026)
- [Supplementary pinned README, committed November 22, 2026 at 19:59:12 Beijing time, after the candidate](https://github.com/EL4CTEO/fast-anything/blob/ebc04b09aabad2b759d7791d4d0c997e0a9fbd01/README.md)

[中文](../fast-anything-ai-hot-function-rust-replay-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
