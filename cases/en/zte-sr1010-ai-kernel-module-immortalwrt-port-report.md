# ImmortalWrt on the ZTE SR1010: a report of AI-assisted closed-module research and driver rewriting

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: Needs verification

At 19:50:49 Beijing time on November 23, 2026, EnoTZ (@EnoTZ2009) introduces an ImmortalWrt port for the ZTE Nebula MAX SR1010, describing a dual-core 1 GHz ZX279133, 512 MB RAM and five 2.5G ports. The poster relays the porter's claim that there is no public chip manual or SDK and the vendor kernel is closed, so AI helped read original kernel modules and progressively rewrite drivers in mainline style. The goal is an alternative system for this device, not merely AI following existing flashing instructions.

The post reports a 1.2.0 release based on ImmortalWrt 25.12, installable through the vendor web updater's package format, with dual firmware slots allowing return to the original configuration. It also claims hardware offload, WireGuard, ZeroTier, dae and roughly 700 Mbps multicast under PPPoE. These remain secondhand claims. The porter's original report, code, module addresses, build logs, hardware tests and rollback verification were not obtained. A formal-release label does not establish upstream acceptance or eliminate bricking risk. Retrieval confirms the introducing poster, not a model or REA stack. No firmware was downloaded, device connected or flashing performed. Status remains unverified; the roughly 230-yuan price is the post's historical account, not a current quote.

Sealed snapshot: 0 likes, 27 views, 0 reposts, 0 replies. Version, rollback and performance are secondhand reports, not tested here.
A new secondary account at 22:09:56 Beijing time on November 23, 2026 adds network, switch-chip and flash drivers rewritten with AI from vendor modules, Linux 6.18 with ImmortalWrt 25.12, 128 MB NAND and an eight-core/64-thread NPU. It repeats retention of the original system in dual slots. Nebula MAX is the same SR1010, not a new entry. The porter's code and verification records remain unavailable, so simple flashing is not accepted as safe. Sealed candidate: 43 likes, 5,598 views, 2 reposts, 1 reply.

## Sources

- [EnoTZ introduces SR1010 AI-assisted driver rewriting and firmware, November 23, 2026 at 19:50 Beijing time](https://x.com/i/status/2124833044599120153)
- [Secondary account of Nebula MAX driver scope and Linux version, November 23, 2026 at 22:09 Beijing time](https://x.com/i/status/2124868051468440014)

[中文](../zte-sr1010-ai-kernel-module-immortalwrt-port-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
