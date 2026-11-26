# Real2SimLab: a unified platform scoring video-to-simulation programs with benchmark protocols

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-27
Stage: Analysis test

At 03:19:19 Beijing time on November 27, 2026, Zefan Cai (@Zefan_Cai) introduces Real2SimLab, connecting methods that reconstruct simulation programs from recordings of physical events to multiple benchmarks. It aims to avoid pairwise method/benchmark integrations and scoring drift from rewritten evaluators. The post reports forty-seven coding agents, five non-agent methods and six benchmarks, and says training/reward pipelines filter overlapping evaluation recordings before using the same scoring code.

Supplementary reading of Real2SimHub/Real2SimLab's README finds HEAD 1c36025f79f9f071fc419adb37166a8aefc3efdf, dated November 26, 2026 at 08:46:51 UTC, before this window. The docs describe generating programs reproducing physical events from video, then freezing delivered artifacts, rerunning them offline/read-only and scoring each benchmark under its own protocol. The forty-seven agents are Harbor 0.27's supported range, with five also directly integrated, not evidence that all forty-seven completed every benchmark in this report. Raw IRIS data and the project's own synthetic suite use Lab metrics, so not every score is a third-party official score.

The documentation proposes excluding identical files/recordings from training exports and describes sandbox/network limits. These are project statements, not a security audit, proof of no leakage or unique identifiability of every physical parameter. Full results, implementation and paper were not reviewed; dependencies, agents and simulations were not run, and scores were not recomputed. Included as an evaluation tool for broader AI-assisted behavior/physical reconstruction, with REA unmentioned. Coverage counts are not accuracy.

Sealed candidate: 0 likes, 13 views, 0 reposts, 0 replies. 47/5/6 are reported coverage counts, not measured accuracy.

## Sources

- [Zefan Cai introduces Real2SimLab, November 27, 2026 at 03:19:19 Beijing time](https://x.com/i/status/2126033076006646034)
- [Pre-window supplementary README, HEAD at reading: 1c36025 dated November 26, 2026 at 08:46:51 UTC](https://github.com/Real2SimHub/Real2SimLab/blob/1c36025f79f9f071fc419adb37166a8aefc3efdf/README.md)

[中文](../real2simlab-agent-simulation-benchmark-pipeline.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
