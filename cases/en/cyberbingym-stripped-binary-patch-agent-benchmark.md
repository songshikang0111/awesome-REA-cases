# CyberBinGym: patched binaries help agents recover bugs, but 88% recovery is not 20% exploitation

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-11
Stage: Analysis test

At 09:01:59 Beijing time on November 11, 2026, 心有猛虎 (@zg0820) introduces CyberBinGym: whether AI can infer vulnerabilities from released binary patches and exploit a controlled service, rather than merely explain code. Another candidate at 10:41:46 adds six vulnerability families, three analysis-complexity levels and human trajectory auditing. The 11:32 post repeats that text verbatim, not a new experiment.

Supplementary reading covers the abstract and submission record of arXiv:2611.10723v1, by Lambang Akbar Wijayadi, Zhaoqi Xiao, Zhun Wang, Hongwei Li, Wenbo Guo, Heng Yin, Zhenkai Liang and Dawn Song. Version 1 was submitted November 7 at 13:31:11 UTC, or 21:31:11 Beijing time, before this window. The candidate's November 10 release date does not overwrite the original submission date. Only the abstract page was read, not the full paper, task implementation or trajectories.

The abstract confirms 100 tasks from real vulnerabilities in 53 widely used projects, spanning six families and three complexity levels. Agents receive stripped vulnerable and patched binaries without source or vulnerability information and combine static/dynamic analysis. Evaluation separates recovery through differential crash testing from end-to-end exploitation through flag retrieval, auditing trajectories to reject reward hacking. The strongest agent reportedly recovers 88% and exploits 20%. On a matched 20-task subset, the patched binary raises exploitation from 10% to 25%. With standard binary hardening, two of the 20 previously successful tasks remain exploitable. Different denominators and conditions cannot be combined into a universal success rate.

The candidate attributes the three configurations to Codex/GPT-5.6 at 88% and 20%, Claude Code/Opus 5 at 85% and 6%, and Kimi Code/K3 at 64% and 0%. The abstract does not enumerate models, so exact configurations and the latter two pairs remain attributed to the candidate, without checking paper tables. The candidate also describes runtime dependencies, analysis tools and a controlled victim, withholding reference PoCs and source patches. No patch source does not mean no patched binary. The study does not establish exploitation of arbitrary production targets or exclude prior training exposure to open-source projects. REA is unmentioned. This collection executed no vulnerable samples, contacted no victim and reran no exploits.

The two sealed candidates respectively have 3 likes/371 views/0 reposts and 0 likes/94 views/0 reposts. Metrics are research reports, not reproduction by this collection.

## Sources

- [Candidate: 心有猛虎 on CyberBinGym and three configurations, November 11, 2026 at 09:01:59 Beijing time](https://x.com/i/status/2120321105240240426)
- [Supporting candidate: six families, three levels and trajectory auditing, November 11, 2026 at 10:41:46 Beijing time](https://x.com/i/status/2120346216110096572)
- [Supplementary original v1 abstract/submission record, November 7, 2026; pre-window material](https://arxiv.org/abs/2611.10723v1)

[中文](../cyberbingym-stripped-binary-patch-agent-benchmark.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
