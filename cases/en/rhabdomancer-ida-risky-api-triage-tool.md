# rhabdomancer v1: marking potentially risky API calls in IDA for further investigation

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Related project

At 06:37:01 Beijing time on November 17, 2026, Takashi Yoshikawa (@MalwareBibleJP) summarizes Hex-Rays' v1 introduction for haruspex, rhabdomancer and augur. The independent role of rhabdomancer is displaying potentially risky API call sites in an IDA analysis database, focusing researchers on suspicious code before closer LLM examination and human static/dynamic validation.

Supplementary reading covers Marco Ivaldi's Hex-Rays author article published November 12, 2026 at 19:52:28 UTC and rhabdomancer's README pinned at ffed414, committed November 16 at 09:11:44 UTC, both pre-window evidence. The docs confirm call sites printed to stdout and marked in the IDB, three priority tiers and configurable API lists. The article places deeper LLM triage before human confirmation and credits Claude with helping write tests. Its 280 AArch64 ELF binaries totaling 14 MB take 356 seconds with old v0.9.3/IDA 9.3 versus 342 seconds with v1.2.0/IDA 9.5 on the same MacBook Air M3, starting without IDBs and including initial analysis. Tool and IDA both change; their effects cannot be isolated.

A dangerous API call is not automatically an exploitable flaw, nor is the tool an autonomous LLM agent. Function exports belong to haruspex, while string associations and the 39.3-minute/124-second result belong to augur; performance is not transferred. Stronger LLM integration and LibAFL automatic confirmation remain plans. Only posts, the author article and pinned README were read, not full source, configuration rules or results. Neither IDA nor targets were run. REA is unmentioned; status remains related-project.

The shared three-tool candidate has 4 likes, 414 views, 1 repost and 0 replies at sealing. This is not a separate rhabdomancer test or vulnerability count.

## Sources

- [Takashi Yoshikawa relays Hex-Rays' three-tool v1 account, including rhabdomancer API-call marking, November 17, 2026 at 06:37:01 Beijing time](https://x.com/i/status/2122458950763499685)
- [Pre-window supplement: Marco Ivaldi's audit pipeline and combined-version comparison, November 12, 2026 at 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [Pre-window supplement: pinned rhabdomancer README, committed November 16, 2026 at 09:11:44 UTC](https://github.com/0xdea/rhabdomancer/blob/ffed41482fd650e86b1256ae70146e5247aa8932/README.md)

[中文](../rhabdomancer-ida-risky-api-triage-tool.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
