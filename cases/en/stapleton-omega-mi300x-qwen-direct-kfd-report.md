# Omega runs Qwen on MI300X: Stapleton reports direct kfd access without AMD's user-space runtime

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-16
Stage: Needs verification

At 07:07:59 Beijing time on November 16, 2026, an open letter describing Michael Drake Stapleton's research lists 'Omega running Qwen3.8-27B on an AMD Instinct MI300X' (Zenodo 24237047), presented as a technical brief for the UXL Open Source Working Group. This target is model execution on AMD MI300X, separate from the letter's NVIDIA GB10/CUDA++ target, not another CUDA-compatible implementation.

According to the letter, on November 13, 2026 an Omega-language program ran Qwen3.8-27B-FP8 on MI300X with no AMD user-space runtime in the process, communicating directly through /dev/kfd. Its published median decode time was 26.7 milliseconds per token. A subsequent November 14 session reached 16.226 milliseconds per token, but that optimized build had not landed in the public clone; the letter explicitly distinguishes the evidence status. These dates predate the candidate and identify reported historical runs, not new tests in this window. No inference is made that kernel drivers are unnecessary, arbitrary AMD cards work, model outputs are fully correct or this measures end-to-end throughput.

The letter places the overall work within human-directed agent development across GPU stacks and model runtimes but gives no model, agent task allocation, source commit or test configuration for this particular path. Neither the brief, clone nor measurement records were read. The supplementary Zenodo API request returned 403; its record number only traces the letter's citation. This collection ran no model and accessed no GPU. The account remains attributed and unverified; the unpublished faster build is not presented as reproducible performance, and the letter's legal claims are not adjudicated.

Sealed candidate: 1 like, 71 views, 0 reposts, 0 replies. Both 26.7 and 16.226 ms/token come from the letter; the latter build was not public.

## Sources

- [Open-letter Omega/MI300X execution account and two evidence stages, November 16, 2026 at 07:07:59 Beijing time](https://x.com/i/status/2122104354140205554)
- [MI300X technical brief 24237047 cited by the letter; text not obtained, API returned 403](https://zenodo.org/records/24237047)

[中文](../stapleton-omega-mi300x-qwen-direct-kfd-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
