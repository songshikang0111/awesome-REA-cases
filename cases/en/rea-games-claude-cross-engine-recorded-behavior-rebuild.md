# rea-games: Claude rebuilds open-source games across engines and compares recorded behavior frame by frame

Category: Games and preservation · REA use unconfirmed
Record date: 2026-11-25
Stage: Needs verification

At 15:59:03 Beijing time on November 25, 2026, erKam (@erkamyaman_ng) introduces rea-games: give Claude an open-source game, rebuild it in another engine and compare behavior frame by frame. The root post claims every recorded frame matches for 2048, Chrome Dino and Canvas Bird in web, Rust and Godot versions. They are examples of one rebuilding tool, not three independent tool projects. The objective is preserving existing game behavior rather than generating a visually similar interface from screenshots.

The author's 15:59:41 reply says 2048 reuses the same moves and random numbers across 19 games and 24,044 inputs, with matching boards after each move. Changing new-tile odds from 0.9 to 0.8 leaves only 3 of 19 passing. This negative control attempts to test the comparator's ability to detect changed behavior, not all seeds, inputs or implementations. The 15:59:58 reply reports 29 Chrome Dino recordings and 63,000 frames, illustrating 1,800 steps, 23 obstacles, a pterodactyl and then a crash, comparing obstacle positions, dino height, crash and score. Matching logical state is not pixel identity or a mathematical proof over all gameplay. These replies supplement the earlier window; they are not new candidates in this review.

This window's new 18:17:04 candidate further describes recording original inputs, random numbers and state, writing a GAME.md mechanics specification, rebuilding in Godot, Rust/Bevy or the web, then replaying the same inputs to locate state differences. It adds Blocks as a fourth example and broadly claims hundreds of thousands of matching inputs and frames. This is a secondary project introduction without separate Blocks counts or check records. It neither extends the original author's finite validation coverage nor constitutes independent reproduction.

Source code, raw recordings, harness, comparison definitions and separate Canvas Bird/Blocks validation were not read, and nothing was built or rerun. The rea name does not establish use of morluto/rea; rea remains unknown. Any game and any engine describe ambition, not verified coverage. Status is unverified; every figure and result retains author or secondary-writer attribution.

Sealed root post: 0 likes, 1 view, 0 reposts, 1 reply. Engagement does not establish result credibility; reply figures were not independently rerun.
18:17 secondary candidate: 38 likes, 746 views, 4 reposts, 2 replies in the sealed snapshot. No new raw validation logs.

## Sources

- [erKam introduces rea-games and cross-engine recorded comparisons, November 25, 2026 at 15:59:03 Beijing time](https://x.com/i/status/2125499490606145735)
- [Supplementary author reply: 19 recorded 2048 games, 24,044 inputs and a probability-mutation negative control, November 25, 2026 at 15:59:41 Beijing time](https://x.com/i/status/2125499651566522513)
- [Supplementary author reply: 29 Chrome Dino recordings and 63,000 frames, November 25, 2026 at 15:59:58 Beijing time](https://x.com/i/status/2125499725050745291)
- [New secondary account: GAME.md, input/state replay and Blocks, November 25, 2026 at 18:17:04 Beijing time; not independent validation](https://x.com/i/status/2125534226636509548)

[中文](../rea-games-claude-cross-engine-recorded-behavior-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
