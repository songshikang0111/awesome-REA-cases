# DecBench: separating structure, type recovery and recompilation similarity in LLM decompilation

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-19
Stage: Analysis test

At 16:30:13 Beijing time on November 19, 2026, yibie lists Noelo Lab's DecBench in a directory update, describing comparisons of decompilers and modern LLMs at exact-source recovery and calling Kuna the leader. The candidate also introduces two separate game projects, recorded separately rather than treating the entire directory as one experiment.

The README at b65837037c7e93dbd3db01e72fa8d46641686dcb was read as supplementary methodology. Its commit is November 11 at 04:38:13 Beijing time, before this window. Metrics include control-flow graph edit distance, type correctness against DWARF, and recompilation with the original toolchain after a compilability fixup, followed by assembly Jaccard similarity with linker-dependent operands normalized. Union counts functions perfect on any one of the three metrics, not all three simultaneously or whole-binary byte identity.

Documentation provides a public dataset and a 250-function external-entry sample. It says much code is coding-agent-generated, but humans own and take responsibility for the core ideas and submissions; fully autonomous contributions are not allowed. Complete metric implementations, the live leaderboard and per-function results were not read, so Kuna's current first place is unconfirmed and 137 stars is not adopted as verified engagement. The benchmark was not run. Retained as analysis-test for bounded function metrics, not proof AI recovered all original source; REA is unmentioned.

## Sources

- [yibie's DecBench and two-game directory update, November 19, 2026 at 16:30:13 Beijing time](https://x.com/i/status/2123333006870131110)
- [Supplementary pinned DecBench README, commit November 11, 2026 at 04:38:13 Beijing time](https://github.com/Noelo-Lab/decbench/blob/b65837037c7e93dbd3db01e72fa8d46641686dcb/README.md)

[中文](../decbench-llm-decompiler-exactness-benchmark.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
