# MiniMax's internal decompiler experiment: reinserting a Rust core into the original host

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-28
Stage: Analysis test

Candidates at 21:45:00 and 21:47:11 Beijing time on November 28, 2026 relay MiniMax's internal software-protection evaluation. The latter, by Hard Signal (@cccc2024cccc), names the report in Chinese as '重新思考软件保护的新范式' and identifies the target as an unnamed closed-source decompiler, a tool translating machine code into readable pseudocode. No product or vendor is guessed.

According to Hard Signal, the unreleased strongest internal model received Ghidra, GDB, a test framework, compiler and custom multi-agent harness. It divided tasks itself and compared original and Rust-rewritten modules on the same samples. Reported totals are 2,000 subagent sessions, roughly two million lines of experimental code and 10,000 automated tests. The line count covers exploration, not final product size or a claim that every line was useful.

The more concrete check reportedly compiled the rewritten core into a shared library and replaced the library in the original program's directory, preserving its interface. The host allegedly still started, loaded files and decompiled them. This supports the described interface-compatibility experiment, not a complete clone, equivalence on every input, unique recovery of original source or complete feature acceptance. The later post explicitly limits the work to a core-module experiment, far from a mature commercial product and highly dependent on custom scaffolding.

This collection retrieved Hard Signal's post to confirm attribution and full wording, then read MiniMax's original website report, titled 'MiniMax Research：重新思考软件保护的新范式' and dated November 28, 2026. This is supplementary primary evidence, not a new candidate. No publication time is given, so publication within this strict window is not established. The original confirms 2,000 sessions, roughly two million experimental lines, 10,000 tests and host reinsertion. It distinguishes three internal checks: CLI/API calls to the core pipeline comparing sample outputs and timings; a separate lightweight UI for browsing functions and pseudocode; and shared-library replacement preserving the original GUI. It reports some analysis-speed improvement without inspectable numerical results; Rust alone does not certify a performance advantage.

The original explicitly limits results to experimental core modules, with major gaps in the surrounding ecosystem, cross-platform UI and long-term stability, and dependence on decomposition and differential-testing scaffolding. Public deployment is not the internal model. The company says evaluation was isolated and that all reconstructed code, build artifacts, scripts and logs were irreversibly destroyed afterward, never distributed or commercialized, and that public capabilities may be restricted. These are company statements, not an independent destruction audit or implemented policy. Samples, source, shared libraries, a complete test inventory and logs were not obtained. The initial end-to-end cloning shorthand is bounded by these limits. This collection read documentation only, running or reproducing nothing. VMProtect/Themida is recorded separately; REA is unmentioned.

Sealed snapshots: first post 2 likes, 157 views, 0 reposts, 0 replies; later post 0 likes, 47 views, 0 reposts, 0 replies. Both relay an internal company evaluation, not two independent experiments.

## Sources

- [Brief account of MiniMax's decompiler core and protected samples, November 28, 2026 at 21:45:00 Beijing time](https://x.com/i/status/2126673716956529120)
- [Hard Signal adds sessions, exploratory code, shared-library replacement and limitations, November 28, 2026 at 21:47:11 Beijing time](https://x.com/i/status/2126674264493613427)
- [Supplementary company report: three internal checks and product/release limits, dated November 28, 2026 with no time](https://www.minimax.cn/blog/minimax-internal-model-reverse-engineering-evaluation)

[中文](../minimax-internal-decompiler-rust-core-replacement-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
