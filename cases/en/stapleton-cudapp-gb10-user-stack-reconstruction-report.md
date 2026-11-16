# CUDA++ and Spark Secrets: Stapleton reports rebuilding parts of the GPU user-space execution stack on GB10

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-16
Stage: Needs verification

An open letter posted at 07:07:59 Beijing time on November 16, 2026 describes Michael Drake Stapleton's research. It presents a human constraining and directing agents across kernels, languages, GPU stacks and model runtimes, while acknowledging uncertain attribution of specific implementation ideas. This entry records only the GPU-target technical account, not judgments about the letter's legal allegations, platform moderation or research validity.

The letter cites 'Reverse Engineering the CUDA Software Stack' (Zenodo 23677465), describing CUDA++ as a research-stage GPU machine-code toolchain for NVIDIA GB10. It reportedly avoids NVIDIA's proprietary user-space compiler, runtime, driver library and mathematics libraries, but still uses NVIDIA's open Linux kernel modules and signed firmware. Claimed archived results include exhaustive GPU/CPU-sequence parity for nine declared FP32 operations and a 1,048,576-element vector add whose code and output hashes match its host-simulator record. A full-chip 1,048,576/1,048,576-value test dated October 22, 2026 is historical background in the letter, not a new run in this window.

For the same GB10 target, 'The Spark Secrets' (listed as Zenodo 24047504) additionally reports barrier-inclusive launch costs of 25.09–31.97 microseconds, 115.14 TFLOPS, 195.1 GB/s, and a 35B model matching 32/32 token IDs on three prompts and 31/32 on a fourth. The letter explicitly scopes these as achieved probe results rather than hardware ceilings and not a complete drop-in CUDA-ecosystem replacement. Single-machine measurement and incomplete token agreement remain important limits.

This collection read the full candidate letter, not the papers or test logs. Supplementary requests to two relevant Zenodo APIs returned 403; no paper text, archived source, hash inventory or agent traces were obtained. The linked record number is a tracing aid, not checked paper content or publication date. Models and REA use are unspecified; AI involvement is attributed only to the letter's human-directed-agent background. No GPU toolchain was run or performance verified. Status remains unverified.

Sealed candidate: 1 like, 71 views, 0 reposts, 0 replies. All GPU figures are project results relayed by the letter, not calculated or reproduced here.

## Sources

- [Open-letter CUDA++/GB10 and Spark Secrets technical account, November 16, 2026 at 07:07:59 Beijing time](https://x.com/i/status/2122104354140205554)
- [CUDA-stack record 23677465 cited by the letter; text not obtained, API returned 403](https://zenodo.org/records/23677465)

[中文](../stapleton-cudapp-gb10-user-stack-reconstruction-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
