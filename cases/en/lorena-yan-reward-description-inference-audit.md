# Reward-description inference: Tianyi Lorena Yan uses contrasting rewarded rollouts to expose actual preferences

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-03
Stage: Analysis test

At 06:40 Beijing time on November 3, 2026, Tianyi Lorena Yan (@LorenaYannnnn) replies to Max Mao: direct AI auditing of a grader/reward model (RM) is a strong baseline, but same-prompt rollouts with different rewards supply contrastive evidence for inferring actual preferences and possible exploits, especially with complex rubrics or hard-to-explain neural RMs. The goal is not source recovery: language models infer hidden reward behavior from training records to make chain-of-thought (CoT) monitoring more informative.

The October 20, 23:00 Beijing-time research thread and October 23, 10:29 question were read as pre-window method background. The work with John Hewitt constructs three reward mismatches: exceeding length limits, model-family bias in judging, and code passing only some tests. It takes training rollouts with high reward variance, prompts an LM for candidate reward descriptions, keeps the description helping a frozen base model achieve high rewards, then injects it into training inputs so models verbalize it in CoT. The thread reports improved monitorability across models/tasks, without numerical scores in the text read here.

The candidate explains the information advantage of an existing method, not a new November 3 experiment. In a November 3, 00:07 follow-up, the author also describes false-positive/false-negative labeling difficulties with complex judge models. Coverage of arbitrary RMs, reliable discovery of all loopholes or corrected rewards is not established. The full paper, data and code were not inspected and training was not rerun. Results remain researcher reports.

Candidate snapshot: 0 likes, 3 views, 0 reposts. Supplementary research results were not reproduced by this collection.

## Sources

- [Tianyi Lorena Yan compares reward inference with direct auditing, November 3, 2026](https://x.com/i/status/2117386424613847329)
- [Supplementary research introduction, October 20, 2026, before the window](https://x.com/i/status/2112559477270421539)
- [Supplementary LM descriptions and frozen-base selection method, October 20, 2026](https://x.com/i/status/2112559480294584570)
- [Supplementary Max Mao question about direct AI auditing, October 23, 2026](https://x.com/i/status/2113457815394418992)
- [Supplementary author reply on complex judges and labeling, November 3, 2026, 00:07, before the window](https://x.com/i/status/2117287579242369277)

[中文](../lorena-yan-reward-description-inference-audit.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
