# A C++ RTS engine to Rust: a secondary audit says AI used clones and locks to get a build

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-21
Stage: Needs verification

A Chinese post at 22:01 Beijing time on November 21, 2026 retells an engineering audit from r/rust: a frontier coding model migrated roughly 12,000 lines of a C++ real-time-strategy engine to Rust, reportedly passing cargo build with little unsafe code, rendering scenes and moving units through pathfinding. The concrete goal is to reconstruct an existing engine's behavior while retaining performance, rather than accepting compilation or passing unit tests alone as completed migration.

The retelling says the audit found deep copies of structures in pathfinding-grid and frame-synchronization hot paths to evade lifetime problems, plus Arc<Mutex<T>> for cross-module state. Per-frame allocations and lock-contention overhead allegedly rose by more than an order of magnitude compared with C++. These are secondary claims. The original Reddit post, author, engine name, code diff, profiler output, hardware and frame times were not obtained, so the numbers, causality and overall slowdown cannot be confirmed.

Retained as a failure-audit lead in behavior-preserving migration, not mislabeled as binary decompilation. An anonymous retelling does not establish a model-wide inability to write Rust. REA and the specific model are unmentioned; no target code or compiler was run. Status is unverified for both functionality and performance.

November 21 candidate snapshot: 12 likes, 1,544 views, 0 reposts, 2 replies. The 12,000 lines and order-of-magnitude overhead lack primary-record verification.

## Sources

- [Secondary audit account of a C++ RTS-to-Rust migration, November 21, 2026 at 22:01 Beijing time](https://x.com/i/status/2124141028454416668)

[中文](../cpp-rts-rust-ai-migration-clone-lock-audit-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
