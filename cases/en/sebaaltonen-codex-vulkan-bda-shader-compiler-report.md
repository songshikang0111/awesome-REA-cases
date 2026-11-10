# Vulkan BDA shader compilers: Sebastian Aaltonen links Codex-assisted reversing to GPU-pointer problems

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-10
Stage: Needs verification

At 15:49:47 Beijing time on November 10, 2026, Sebastian Aaltonen (@SebAaltonen) says Codex (Astra Ultra) is excellent at reversing and associates Intel and AMD shader-compiler bugs with GPU pointers and Vulkan BDA. BDA means Buffer Device Address, allowing shaders to access buffers through device addresses. This records the author's short analysis connecting AI reversing capability to a concrete graphics-compiler problem, not a general model ranking.

He contrasts DX/OpenGL buffer abstractions with pointers in Metal, CUDA and OpenCL, saying Vulkan 1.3+ supports both. These API generalizations remain attributed to him and were not checked version by version here; they do not establish that an API never offers pointers or that all drivers share a defect. The post supplies no particular shader, input/output, disassembly, prompt, compiler version, driver, hardware or reproducer, and does not show exactly what Codex analyzed.

Supplementary retrieval confirms attribution, text and an image attachment, not its content or the quoted original. No issue, fix commit or vendor confirmation was obtained. The word bug does not establish an exploitable security vulnerability, settled root cause or delivered fix. Performance and cross-vendor consistency were not measured. Retained as unverified author analysis. REA is unspecified; no GPU workload or target code was run.

Sealed candidate: 8 likes, 327 views, 0 reposts. No driver version, minimal reproducer or independent validation.

## Sources

- [Sebastian Aaltonen on Codex and Intel/AMD Vulkan BDA problems, November 10, 2026 at 15:49:47 Beijing time](https://x.com/i/status/2120061340899541291)

[中文](../sebaaltonen-codex-vulkan-bda-shader-compiler-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
