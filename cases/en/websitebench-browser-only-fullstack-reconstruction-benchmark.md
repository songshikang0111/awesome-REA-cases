# WebsiteBench: browser-exploration full-stack reconstruction tested against hidden behavior and visual checks

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-15
Stage: Analysis test

At 06:02:13 Beijing time on November 15, 2026, Johnnysama (@JohnnyS03832498) introduces WebsiteBench: agents explore production-level websites through a browser and rebuild full-stack implementations matching appearance and behavior, not just screenshots. Supplementary research located TIGER-AI-Lab/WebsiteBench and read the README pinned at 3868d82d137f4ff8f5b2bd858ed8c279da3aeda1, committed November 10, 2026 at 06:47:19 UTC, before this window. It supports methodology, not another candidate or results produced here.

Documentation lists 70 websites and 46,916 hidden test cases, with 302 to 2,016 per task. A case passes only when functional checks pass and every visual checkpoint reaches normalized SSIM of 0.99. Task reward is the share of passing cases, not the probability that an entire website has been fully cloned. Harbor execution and reference-solution checks are documented; this collection installed no dependencies, downloaded no tasks and ran no benchmark.

The candidate reports Opus 5.5 at 26% hidden-test passes and 71% at the request level, Amazon at 56.8% and LeetCode as high as 74.2%. It gives DeepSeek V4.1 Flash 13.5% at $4.6 per task, versus $305 for Opus. These are the commentator's snapshot. The read README supplies no model leaderboard, request-metric definition, cost accounting or per-site results, so they remain unverified here. The percentages cannot be conflated, interpreted as complete cloning or used to calculate a comparable cost reduction. No actual REA use is established; absence of an extra harness is the commentator's inference.

The README licenses benchmark code, task definitions and verifier under Apache-2.0, while third-party reference-site content retains its owners' rights and is for non-commercial research only. Full licensing and reference implementations were not reviewed; production-site redistribution rights are not implied. Included as AI-assisted black-box functionality reconstruction with a public evaluation method, not independently reproduced results. Findings remain attributed to the project or commentator.

Sealed candidate: 2 likes, 72 views, 0 reposts, 1 reply. 26% and 71% are different metrics; model versions, costs and per-site results were not checked against raw results.

## Sources

- [Johnnysama introduces WebsiteBench and model scores/costs, November 15, 2026 at 06:02:13 Beijing time](https://x.com/i/status/2121725416557908217)
- [Pre-window pinned README: task scale, SSIM scoring and licensing, committed November 10, 2026 at 06:47:19 UTC](https://github.com/TIGER-AI-Lab/WebsiteBench/blob/3868d82d137f4ff8f5b2bd858ed8c279da3aeda1/README.md)

[中文](../websitebench-browser-only-fullstack-reconstruction-benchmark.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
