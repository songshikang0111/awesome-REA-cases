# LiberNT: AI-assisted Windows 11 black-box compatibility research, still a test pre-release

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-21
Stage: In progress

At 02:18:46 Beijing time on November 21, 2026, HKEPC (@hkepcmedia) introduces LiberNT, a free NT operating system targeting Windows 11 compatibility. The report credits AI with studying low-level behavior, writing and reviewing code, and describes required human review and end-to-end validation. The aim is running Windows applications on modern hardware, not recovering original Windows source. The report claims wins in 112 of 132 performance comparisons, over 2,000% in some, and a worst deficit of about 28%. Corresponding environments and raw results were not obtained or rerun here; none is this collection's performance finding.

Supplementary public-repository reading covers README and AGENTS at 0542ae580c1d36b5fb226aa4cf9fdacce030cbdf, whose committer date is November 19 at 02:58:01 Beijing time, before this window. Reading on November 21 supplies identity, methodology and limits, not another candidate. README explicitly says AI reads documentation, extracts definitions and compares Microsoft Learn requirements with the project's functions. It says humans review generated code and run end-to-end tests before merges. Sources include SDK/WDK headers, Windows 11 public symbols, Microsoft documentation and black-box runs. Rules require comparing individual checks from the same tests on Windows 11, and prohibit transcribing disassembled/decompiled Windows code into implementations. Rules do not prove each test was performed; full test logs were not audited and the system was not run here.

Docs identify a ReactOS fork with most of the tree still shared, listing new memory/cache management, ARM64, WoW64, graphics and device work. The media's new-kernel wording is not evidence the entire system was rewritten from scratch. README lists amd64, arm64 and riscv64 images and i386 source builds; AGENTS at the same revision still describes RISC-V64/PPC as in progress. An image list is not complete feature parity on every architecture. Release builds are explicitly Debug pre-releases for testing, not a computer users depend on. The report's REA name is not confirmed by the docs as the morluto/rea tool, so classification is other-ai and in-progress. No images were downloaded, dependencies installed or targets run, and compatibility, performance and legal compliance were not independently verified.

Sealed candidate: 12 likes, 844 views, 4 reposts, 0 replies. Performance figures come from the report, not measurements by this collection.

## Sources

- [HKEPC's LiberNT report, November 21, 2026 at 02:18:46 Beijing time](https://x.com/i/status/2123843509157539992)
- [Supplement: pre-window README pinned November 19 at 02:58:01 Beijing time, AI methodology and pre-release limits](https://github.com/LiberNT/LiberNT/blob/0542ae580c1d36b5fb226aa4cf9fdacce030cbdf/README.md)
- [Supplement: AGENTS at the same revision, source rules, ReactOS relationship and Windows 11 comparison requirements](https://github.com/LiberNT/LiberNT/blob/0542ae580c1d36b5fb226aa4cf9fdacce030cbdf/AGENTS.md)

[中文](../libernt-ai-windows11-blackbox-compatibility.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
