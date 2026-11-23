# Mjolnir: project-grounded agents investigate root-of-trust firmware and RTL vulnerabilities

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: Analysis test

At 12:19:22 Beijing time on November 23, 2026, @gastronomy posts a research abstract for Mjolnir targeting six root-of-trust firmware and RTL targets in Caliptra, OpenTitan and OpenPRoT. Roots of trust underpin secure boot and attestation. Relevant bugs may depend on project-specific trust boundaries and fault-injection countermeasures without causing crashes, making generic vulnerability patterns insufficient. This is recorded as AI-assisted investigation of hardware/firmware security behavior, not recovery of original source from binaries.

The abstract describes providing project threat models and design conventions to discovery and skeptical-review agents, then reproducing surviving findings through PoC tests in the original project's toolchain. Without physical RoT hardware, agents exercise inputs through hardware models, mocks or RTL testbenches. Project-level reproduction is not equivalent to physical fault-injection validation.

For Caliptra runtime firmware, the abstract reports 83.3%–100% precision across three models under blind expert labeling. Gemini 3.8 Flash reportedly reaches 100%, versus 66.7%–78.6% for four single-agent baselines using the same model. On 34 known core-firmware security bugs fixed after model training cutoffs, Gemini 3.8 Flash finds 10 versus 7 for the best baseline; Gemini 4 Argon finds 17 versus 12. These are precision and recovery counts for particular evaluations, not accuracy across every target or recall of all vulnerabilities.

The abstract also claims maintainers confirmed 64 previously unknown security-relevant findings: 37 across three models on Caliptra runtime firmware and 27 across single scans of the other five targets. The paper, model configuration, individual findings, deduplication rules, maintainer confirmations and PoC logs were not obtained. The confirmation count therefore remains attributed to the abstract rather than an independent audit conclusion. Original-thread retrieval confirms the account and text; the short link was not expanded. REA is unmentioned, and no firmware, RTL, target code or tests were executed here.

November 23 sealed candidate: 1 like, 77 views, 0 reposts, 0 replies. Six targets and 64 confirmations are research-abstract figures, not independently reproduced.

## Sources

- [Mjolnir research abstract posted by @gastronomy, November 23, 2026 at 12:19:22 Beijing time](https://x.com/i/status/2124719429686632736)

[中文](../mjolnir-root-of-trust-project-grounded-agents.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
