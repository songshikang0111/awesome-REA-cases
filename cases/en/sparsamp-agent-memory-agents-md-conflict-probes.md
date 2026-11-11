# AGENTS.md versus memory: Sparshith's small black-box probes of Claude Code and Codex priorities

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-11
Stage: Analysis test

At 23:00:00 Beijing time on November 11, 2026, Sparshith Sampath (@SparSamp) reports local headless experiments to infer how Claude Code and Codex resolve conflicting agent-written memories and human-written AGENTS.md. Reported models are Opus 5.5 and gpt-6.1-sol, with five runs per setup. This is black-box behavioral analysis, not binary decompilation. REA is unmentioned.

Experiment one puts opposing CSV/JSON preferences in memory and the file, then swaps them, asking for format, reason and relied-on sources. The author says both tools favor AGENTS.md in all runs. Experiment two fixes CSV in the file and JSON in memory, comparing same-day records and either side stale by 15 days. Codex reportedly continues following the file; Claude identifies staleness and chooses the fresher memory. Experiment three contrasts approval for every paid run with no approval below $5, asking about a $3 evaluation. Codex reportedly follows the file, while Claude always chooses the safer ask-first option.

These conclusions concern the author's small experiment and answers, not verified paid execution, all context-conflict rules or permanent product policy. The author plans to vary prompts and injected context to separate harness and model effects. Exact CLI versions, full run sets and raw logs are absent. This collection did not inspect the three image attachments or rerun the experiments. Five runs per setup is not rewritten as five total; no total is computed from an unspecified setup count.

Sealed candidate: 2 likes, 79 views, 0 reposts. Five runs per setup, 15 days and $3/$5 are author-described experimental conditions, not independently rerun.

## Sources

- [Sparshith's three conflict-priority experiments and caveats, November 11, 2026 at 23:00:00 Beijing time](https://x.com/i/status/2120531998116900881)

[中文](../sparsamp-agent-memory-agents-md-conflict-probes.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
