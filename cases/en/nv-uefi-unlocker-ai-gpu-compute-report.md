# nv-uefi-unlocker: reported AI-assisted GPU research and a Rust pre-driver

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-01
Stage: Needs verification

At 01:56:45 Beijing time on November 1, 2026, HKEPC reports AI assistance with nv-uefi-unlocker, a Rust UEFI pre-driver that sets NVIDIA GPU state before the operating system loads, then hands control back to the system bootloader. The report describes SEC2 scrubbing, FWSEC/WPR2, a signed Booter and a V67 four-write payload, claiming no vBIOS flash or driver modification and restoration after power loss. This report supplies the AI attribution, without naming a model or isolating its contribution.

It cites RTX 4060 Laptop FP16 GEMM rising from 29.89 to 49.33 TFLOPS, RTX 3060 gains of 58–85%, and RTX 2070 FP32-accumulation GEMM rising from 36 to 60–63 TFLOPS. These are reported project/community figures, not guarantees for every GPU under one workload. Supplementary reading inspected README commit 2d68d2eb6cc27fd9c8cc437e4a4872acdd179444, dated October 31, 2026, 19:42:47 UTC, after the candidate but still within the window. It explicitly inherits transaction-chain work from gpu-unlock and gpu-unlock-ada and cites NVIDIA's public kernel modules and prior Turing research. AI cannot be credited with discovering all mechanisms from scratch.

That README lists GTX 16 as theoretically compatible and Pascal or earlier, GA100 and RTX 50 as unsupported; some RTX 20 models retain known issues. It offers disabling Secure Boot or self-signing/trusting a certificate, warns to fully power off after failures rather than retry in the same session, and notes that additional power controls can exceed stock thermal/electrical envelopes. Avoiding vBIOS flashing is not risk-free, and correct firmware hashes do not prove runtime safety. Only reporting and documentation were read: no release binaries downloaded, firmware or Secure Boot changed, or GPU tests run. Gains, AI contribution, compatibility and recovery remain independently unverified.

Candidate snapshot: 16 likes, 961 views, 3 reposts.
AI attribution comes from reporting; no model name or independent GPU retest.

## Sources

- [HKEPC's AI-assisted UEFI-tool report, November 1, 2026](https://x.com/i/status/2116590211350335552)
- [Supplementary first-party post-candidate, in-window pinned README: prior work, compatibility and risks](https://github.com/physicsdolphin/nv-uefi-unlocker/blob/2d68d2eb6cc27fd9c8cc437e4a4872acdd179444/README.md)

[中文](../nv-uefi-unlocker-ai-gpu-compute-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
