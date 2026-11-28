# nvdriver: Eric Hartford credits REA for V100 driver research; the project reports a Rust rebuild and hardware comparisons

Category: Hardware and interoperability · REA
Record date: 2026-11-28
Stage: In progress

At 05:29:12 Beijing time on November 28, 2026, Eric Hartford (@QuixiAI) introduces QuixiAI/nvdriver. Unable to use NVIDIA's open driver on V100s, he reverse-engineers it to gain control of driver behavior and explicitly thanks morluto's REA. He says he fixed it and attributes restrictions on older hardware to a push for upgrades. That commercial motivation is his interpretation, not verified vendor intent; lack of support is not automatically deliberate throttling.

Supplementary reading uses commit 6543601569a1af4a9da65b84ec458ba65635caeb, dated 07:59:02 Beijing time that day. Its README describes reconstructing a no_std Rust kernel core with a small Linux C adapter against NVIDIA 580.178.04's nv-kernel.o_binary, targeting behavioral, register and ABI compatibility with unmodified CUDA userspace and stock companion modules. It reports 82 Unicorn binary oracles, 2,096 controls and 6,288 multi-state cases, plus stock-driver comparisons on eight physical Tesla V100-SXM2-32GB cards in disposable VFIO VMs, claiming no differences for CUDA, PyTorch/NCCL, llama.cpp and other workloads. An oracle here uses the original binary's execution as a reference, not an independent audit.

A four-GPU PyTorch report at the same commit marks passed, device_count 4 and device_name Tesla V100-SXM2-32GB, listing PyTorch 2.5.1+cu124, cuDNN 9.1.0, NCCL 2.21.5, collective digests and clean_unload=true. This is a project-submitted record; its environment and stock comparison were not checked through execution here. The support matrix labels Maxwell, Pascal and Turing through Blackwell as offline HAL/Unicorn checks; non-Volta and display-attached hardware still need live testing, and Tegra is unsupported. Different README sections also retain different offline-check counts; no single total establishes all-path coverage. Status remains in progress, without claiming every GPU works, complete feature equivalence or production safety. No driver was installed, kernel module loaded, target binary downloaded or repository code executed here.

November 28, 2026 sealed candidate: 21 likes, 2,403 views, 5 reposts, 1 reply. Repository validation figures are project reports, not reproductions by this collection.

## Sources

- [Eric Hartford's V100/REA research account, November 28, 2026 at 05:29:12 Beijing time](https://x.com/i/status/2126428149378388330)
- [Supplementary pinned README: support matrix, validation and limitations; commit November 28, 2026 at 07:59:02 Beijing time](https://github.com/QuixiAI/nvdriver/blob/6543601569a1af4a9da65b84ec458ba65635caeb/README.md)
- [Four-GPU PyTorch/NCCL project report at the same commit, not independently rerun](https://github.com/QuixiAI/nvdriver/blob/6543601569a1af4a9da65b84ec458ba65635caeb/reports/final-7cd1-pytorch-nccl-4gpu-rust.json)

[中文](../quixiai-nvdriver-v100-rea-rust-driver-research.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
