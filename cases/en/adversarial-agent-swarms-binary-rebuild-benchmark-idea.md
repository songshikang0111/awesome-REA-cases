# Competitive agent-swarm rewrites: an idea combining cross-team decompilation, hidden faults and independent judges

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-10-31
Stage: Needs verification

At 03:51:16 Beijing time on October 31, 2026, @EERandomness proposes a competitive multi-agent rewriting experiment. Separate swarms cannot communicate directly; each combines frontier and previous-generation models such as Grok, Claude, GPT-6, DeepSeek and GLM, receives goals in multiple natural languages and code-as-prompts, and independently rewrites an entire codebase. No codebase or existing software is identified. This is a concrete research-method idea, not a completed migration.

Each team's red agents inspect their own code and attack other teams' compiled binaries, sharing purported CVEs in a database. They may decompile opponents' binaries and use findings to improve their own implementation. Independent judges continuously assess feature parity, performance and specification compliance through a public leaderboard. One double agent per team deliberately inserts bugs and reports them only to a judge-private database, helping construct tests and red-team metrics. Injected faults are not discovered vendor vulnerabilities, and the post's CVE terminology does not establish officially assigned identifiers.

The writer also imagines judges adding features progressively to influence architecture and teams revising prompts from metrics, with opponents writing the double agent's prompt. The best result is selected by metrics and the others discarded. The full original was checked for these details, but no execution, cost, sample, test suite, code or ranking is supplied. 'More compute = better outcome' remains an opinion, not an experimental result, and availability of every named model is not assumed. REA is unspecified. This collection started no swarms, decompiled no target and executed no research code.

Candidate snapshot: 1 like, 24 views, 0 reposts. A proposal with no identified codebase, measurements or leaderboard.

## Sources

- [EERandomness proposes competitive swarms and cross-team binary research, October 31, 2026 at 03:51:16](https://x.com/i/status/2116256645051465922)

[中文](../adversarial-agent-swarms-binary-rebuild-benchmark-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
