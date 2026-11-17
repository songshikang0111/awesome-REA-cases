# CMP 170HX unlocking report: Pico 2 voltage-controller access and an AI-written irreversible configuration script

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-17
Stage: Needs verification

At 16:20 Beijing time on November 17, 2026, Tiangong Dagongren (@zZztpqw) relays a claimed replication five days after a CMP 170HX mining-card unlocking method became public. The goal is to restore restricted resources and interconnects. Rather than make a separate board, the reported modifier used an approximately $5 Raspberry Pi Pico 2 and four wires to control an onboard voltage-regulator chip over I2C, spending roughly 15 hours. AI is specifically credited with the final one-time configuration-writing script, not independently discovering the entire hardware mechanism. No model is named and REA is not mentioned.

The post reports recognition of 81920MiB of memory, described as 80GB, 126 compute-unit groups, and restored PCIe 4.0 and NVLink. These are relayed recognition and functionality claims without device logs, performance comparisons, a complete resource inventory or reliability tests examined here. They do not establish performance, firmware or complete feature equivalence to an A100. The modifier's 5–10% trigger hit rate and the project author's approximately 14% are also relayed figures, not one-time-write success rates, production yields or measurements by this collection. Parameters were reportedly checked on limited cards.

The source also cites eBay's lowest asking price rising from $2,800 to $4,400 and an approximately $13,000 November average minimum price for used 80GB A100s. No auditable price sample is supplied, so these are not current-price or economic-return guarantees. The poster warns that a wrong one-time configuration can brick the card; only the high-level case is retained, without programming instructions. Retrieval confirmed the poster and text but did not identify the original modifier, source commit, card or original report. No script was executed, GPU accessed or dependencies installed. This remains an unverified secondary report.

Sealed candidate: 3 likes, 74 views, 0 reposts, 4 replies. Neither engagement nor resource recognition establishes A100 equivalence or safe programming.

## Sources

- [Tiangong Dagongren relays Pico 2 and AI-script CMP 170HX unlocking, November 17, 2026 at 16:20 Beijing time](https://x.com/i/status/2122605660487737556)

[中文](../cmp170hx-pico2-ai-configuration-script-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
