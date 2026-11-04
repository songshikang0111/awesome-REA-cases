# Astra weight inspection: reported Qwen edits, language/game identification and control-policy changes

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-04
Stage: Needs verification

At 07:56 Beijing time on November 3, 2026, Kxians (@xulijian1994) relays alleged MIT research: GPT-6 Astra uses Python to read Qwen3.5-0.8B weights, structure and activations, locates MLP layers 15 and 19 and edits 131,072 parameters, reportedly 0.016%, without conventional gradient training. Reported MATH-500 moves from 7.9% to 48.1% and GSM8K from 13.8% to 67.1%, summarized as roughly sixfold. The interpretation is weakening anomalous repetition-related directions rather than injecting math knowledge. Another test allegedly identifies Python, English and romanized Japanese from three small Transformers' middle weights after removing input/output layers.

An account at 17:45:34 that day names MIT CSAIL doctoral student Rikiya Takehi and team, adding IFEval of 21.0% to 62.3%, token-limit looping answers of 93.0% to 33.1% and only a weak Gemma 3 270M change from 6.8% to 7.0%. It refers to a single MLP layer, conflicting with the earlier two-layer account. Games/diffusion shapes recognized from weights and 0-to-100% cart/game control were mentioned without details.

A new candidate at 22:03:33 expands the same study into identifying Breakout, Pong, Pac-Man and Freeway policies from raw weights; editing 3.5% of a cart policy to reach 100% success; and handwriting Breakout network weights allegedly scoring twenty times a PPO model trained for 500 million steps. It repeats Qwen's 0.016% and 7.9%-to-48.1% figures and claims threefold instruction following. It says all execution logs and edited weights are public, conflicting with the earlier no-public-code account. No paper, logs, weight diff or matching repository was obtained, so these accounts are not reconciled.

These are reported experiments within one weight-understanding study, not multiple verified projects. Earlier lookup only confirmed Kxians's authorship. Researcher, institution, model names, parameter percentages and all scores remain secondary claims. Without samples, seeds, generation lengths and complete costs, general improvement, zero compute or understanding all weights is not established. Neither no-code/no-peer-review nor fully-public claims are exhaustive-search conclusions here. No models were downloaded, weights edited or benchmarks run.

A new news commentary at 08:48:32 Beijing time on November 4, 2026 calls the weight-inspection-only framing misleading, attributing to spaCy creator Honnibal the observation that the Qwen improvement experiment used Python and environmental feedback. Raw-weight identification tasks are distinguished from feedback-driven weight editing. This commentary is not a checked reading of the paper, and no conventional training does not imply zero computational cost. The same post's Willison local identification is a separate experiment, not independent reproduction of the math scores above.

Three November 3 candidates: 2 likes/15 views/0 reposts, 1 like/177 views/0 reposts and 7 likes/1,087 views/0 reposts. November 4 commentary: 2 likes, 276 views, 0 reposts. Counts, percentages, scores, publication status and attribution of the rebuttal remain unverified.

## Sources

- [Kxians's Astra/Qwen weight-research report, November 3, 2026](https://x.com/i/status/2117405418175791402)
- [Earlier supporting account: IFEval, repetition and Gemma comparison, 17:45:34 Beijing time that day](https://x.com/i/status/2117553763271561574)
- [New candidate: four-game identification, 3.5% cart edits and Breakout weight claims, 22:03:33 Beijing time that day](https://x.com/i/status/2117618690212659659)
- [New commentary relaying Honnibal's Python/environmental-feedback rebuttal, November 4, 2026](https://x.com/i/status/2117781005520048168)

[中文](../kxians-astra-qwen-weight-inspection-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
