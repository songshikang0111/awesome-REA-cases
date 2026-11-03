# Eighth-generation Lode Runner AI: REA-based gold-drop prediction misses by two frames, level seven still times out

Category: Games and preservation · REA
Record date: 2026-11-03
Stage: Analysis test

At 17:18:25 Beijing time on November 3, 2026, AI-driven development NextCode (@nangoku100katen) reports an eighth-generation Lode Runner game AI. The author claims no human operations and says REA reads the ROM's counting logic to predict where and when an enemy drops gold. The specific example predicts a drop 198 frames later, at F24241, with an actual drop at F24243—a reported two-frame error.

This studies hidden game counters for automated gameplay decisions, rather than rebuilding the game from scratch. The author explicitly says movement remains the same as generation seven and level seven ends in a timeout. A near-correct drop-time prediction does not establish better routing, collection or level completion. The post labels the work unofficial and its voice synthetic.

Original-post lookup confirms the author and attached video, but ROM revision, code addresses, counter derivation, agent source, control logs and repeated trials were not obtained. Unattended operation and frame numbers remain author reports; frames were not independently recounted and a stable two-frame error is not established. No game was run, ROM downloaded or test reproduced.

November 3 candidate snapshot: 1 like, 20 views, 0 reposts. The 198 frames, F24241/F24243 and level-seven timeout are a single author-reported example.

## Sources

- [NextCode reports REA ROM analysis and eighth-generation AI gold-drop prediction, November 3, 2026](https://x.com/i/status/2117546932302381100)

[中文](../nextcode-lode-runner-rea-gold-drop-prediction.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
