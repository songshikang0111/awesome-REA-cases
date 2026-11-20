# LOCA: logic-cone partitioning for LLM recovery of provably equivalent RTL

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-20
Stage: Analysis test

At 10:24:13 Beijing time on November 20, 2026, Tanat Tonguthaisri (@gastronomy) relays an abstract titled Verified Netlist-to-RTL Recovery with LLM Agents. The target is readable register-transfer-level RTL from anonymized gate-level netlists: word-level operations are spread across many gates, and prompting on a whole netlist often fails. LOCA means LOgic Cone Attack. The abstract describes grouping complete next-state logic for related registers into logic cones, assigning parallel agents to rewrite them and assembling compact RTL.

Of five partitioning methods, the abstract says only grouped cones recover designs. It keeps only RTL proven equivalent to the netlist and measures quality by compression. Recovery reaches 17 of 21 model/design pairs versus 6 for whole-netlist prompting; per-run recovery across models rises from 5% to 74%, with median cost below one dollar on a low-cost model. Metrics with different denominators are not conflated. Compression or equivalence does not establish uniquely recovered original designer source.

Function-preserving obfuscation reportedly does not stop recovery on tested designs, while unknown keys or hidden cell functions prevent proof of original-design recovery. Retrieval confirms the poster. Full paper, author list, model/design inventory, source, proof logs and bills were not obtained. Numbers and limits are attributed solely to the abstract, not paper experiments verified by this collection. No netlists, agents or provers were executed, and REA is unmentioned.

## Sources

- [Tanat Tonguthaisri relays the LOCA research abstract, November 20, 2026 at 10:24:13 Beijing time](https://x.com/i/status/2123603287978955162)

[中文](../loca-llm-logic-cone-netlist-rtl-recovery.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
