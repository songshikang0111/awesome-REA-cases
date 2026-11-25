# rea-games: Claude rebuilds open-source games across engines and compares recorded behavior frame by frame

Category: Games and preservation · REA use unconfirmed
Record date: 2026-11-25
Stage: Needs verification

At 15:59:03 Beijing time on November 25, 2026, erKam (@erkamyaman_ng) introduces rea-games: give Claude an open-source game, rebuild it in another engine and compare behavior frame by frame. The root post claims every recorded frame matches for 2048, Chrome Dino and Canvas Bird in web, Rust and Godot versions. They are examples of one rebuilding tool, not three independent tool projects. The objective is preserving existing game behavior rather than generating a visually similar interface from screenshots.

A supplementary reply at 15:59:41 says 2048 reuses the same moves and random numbers across 19 recorded games and 24,044 inputs, with matching boards after every move. The author intentionally changed new-tile odds from 0.9 to 0.8, after which only 3 of 19 games passed. This negative control shows an attempt to test whether the comparator detects changed behavior, not coverage of all seeds, inputs or implementations. Another reply at 15:59:58 reports 29 recorded Chrome Dino runs and 63,000 frames. An illustrative path spans 1,800 steps, 23 obstacles, a pterodactyl and then a crash, comparing obstacle positions, dino height, crash and score. Matching logical state must not be upgraded to pixel identity or a mathematical proof over all gameplay.

Both supplementary replies are within the window and contextualize the same candidate rather than becoming additional candidates. Source code, raw recordings, harness, comparison definitions and separate Canvas Bird validation were not read, and nothing was built or rerun. The rea name does not establish use of morluto/rea; rea remains unknown. Any game and any engine describe the project's ambition, not verified coverage. Status is unverified; every figure and result is attributed to the author.

Sealed root post: 0 likes, 1 view, 0 reposts, 1 reply. Engagement does not establish result credibility; reply figures were not independently rerun.

## Sources

- [erKam introduces rea-games and cross-engine recorded comparisons, November 25, 2026 at 15:59:03 Beijing time](https://x.com/i/status/2125499490606145735)
- [Supplementary author reply: 19 recorded 2048 games, 24,044 inputs and a probability-mutation negative control, November 25, 2026 at 15:59:41 Beijing time](https://x.com/i/status/2125499651566522513)
- [Supplementary author reply: 29 Chrome Dino recordings and 63,000 frames, November 25, 2026 at 15:59:58 Beijing time](https://x.com/i/status/2125499725050745291)

[中文](../rea-games-claude-cross-engine-recorded-behavior-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
