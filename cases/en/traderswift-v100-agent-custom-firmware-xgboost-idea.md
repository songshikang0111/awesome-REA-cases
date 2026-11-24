# TraderSwift's three V100s: Jignesh Davda considers agent-written firmware for XGBoost research

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-24
Stage: Needs verification

At 13:17:29 Beijing time on November 24, 2026, Jignesh Davda (@JigneshDavda) discusses model chains and compute costs in a long TraderSwift AI post. Full-text reading confirms he describes existing code produced by Claude Code driving one or two Codex instances, plus DeepSeek/Qwen experiments. This is development background, not evidence those models have already reversed a GPU.

Later he proposes a concrete legacy-hardware idea: believing older NVIDIA cards become cheaper when excluded from CUDA firmware releases, and XGBoost still suits them, he wants the agent workflow to rewrite custom firmware. He says three V100s have been purchased for an initial test milestone, while he is still sourcing a server to hold them. XGBoost is a tree-model learning tool; the goal is lower-cost compute for trading-model research, not a demonstrated profitable model.

The post conflates CUDA and firmware without identifying whether drivers, runtimes or onboard firmware need changes. Its wording is preserved, not proof that V100 lost a particular support level or needs firmware rewriting. No target version, binary, compatibility implementation, firmware permissions, tests, throughput or returns are supplied. Three cards are a self-reported purchase, not a deployed cluster or performance result. No trading data, firmware download, target execution or GPU tests were accessed here. REA is unmentioned; this remains an unexecuted idea.

Sealed snapshot: 2 likes, 73 views, 0 reposts, 1 reply. Three V100s are author-reported purchases without firmware or performance results.

## Sources

- [Jignesh Davda's TraderSwift post: V100, XGBoost and an agent/custom-firmware idea, November 24, 2026 at 13:17:29 Beijing time](https://x.com/i/status/2125096443199524919)

[中文](../traderswift-v100-agent-custom-firmware-xgboost-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
