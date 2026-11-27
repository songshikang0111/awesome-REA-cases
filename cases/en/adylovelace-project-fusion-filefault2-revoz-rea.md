# Project Fusion: AdyLovelace reports REA/Ghidra research and a FileFault 2 REVoz PoC

Category: Applications and clients · REA
Record date: 2026-11-28
Stage: Needs verification

At 08:51:03 Beijing time on November 27, 2026, Qυεεn Λδγ Lονεlαcε (@AdyLovelace) introduces Project Fusion, reporting REA, Ghidra and AI Agents research on Abyss and MysticalCore that produced FileFault 2 REVoz on macOS 27.3 AArch64. The earlier post also credits custom local analysis workflows developed with Craft Anything, Cláudio dos Códigos and ChatzinGePeTo. Nicknames are preserved without mapping them to commercial models.

A new post at 00:57:11 on November 28 supplies the previously missing FileVault 2 context. The author says the method was discovered accidentally on June 29, 2021 while testing Roland UA-25EX compatibility on macOS Big Sur, adapted on September 2, 2025 to prevent FileVault 2 activation in macOS 26 Tahoe x86-64 tests, and shared with Universo Hackintosh on November 4 for EFI Base integration. MysticalCore was reportedly created on September 2, 2026, moved to macOS 27 Golden Gate AArch64 on the author's MacBook Air M5 Midnight, and merged with Abyss on November 26 in 27.3 to form the PoC. Abyss is described as the stage causing a KernelKit/KASAN fatal crash. Implementation will not be published: materials are for Kira's Lab internal research and the author's own hardware. System/component names and dates preserve the author's account, not independently checked release history or mechanism.

The new post explicitly names FileVault, so its context is no longer described as entirely unknown. However, the claim of breaking FileVault again does not establish successful decryption, bypassing an already encrypted disk, privilege escalation or a registered vulnerability. Preventing encryption activation differs from cracking existing encryption. Source code, samples, hashes, privilege requirements, tool logs, success criteria and remediation details were not obtained. Images were not examined, no PoC run, target downloaded or system protection changed. Retained as an unverified report without executable attack steps.

Old post, sealed November 27, 2026: 1 like, 53 views, 0 reposts, 0 replies. New post, sealed November 28: 0 likes, 44 views, 0 reposts, 0 replies. Neither a PoC name nor success wording is independent verification.

## Sources

- [AdyLovelace's Project Fusion report and REA/Ghidra attribution, November 27, 2026 at 08:51:03 Beijing time](https://x.com/i/status/2126116558028108138)
- [Same author adds FileVault context, timeline and a non-publication plan, November 28, 2026 at 00:57:11 Beijing time](https://x.com/i/status/2126359694402781459)

[中文](../adylovelace-project-fusion-filefault2-revoz-rea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
