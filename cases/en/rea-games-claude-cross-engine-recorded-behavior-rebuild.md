# rea-games: Claude rebuilds open-source games across engines and compares recorded behavior frame by frame

Category: Games and preservation · REA use unconfirmed
Record date: 2026-11-26
Stage: Needs verification

At 15:59:03 Beijing time on November 25, 2026, erKam (@erkamyaman_ng) introduces rea-games: Claude studies an open-source game, rebuilds it in another engine and compares behavior frame by frame. 2048, Chrome Dino and Canvas Bird are examples of one tool, not independent tool projects. At 15:59:41 the author reports 19 recorded 2048 games and 24,044 inputs with matching boards; changing new-tile odds from 0.9 to 0.8 leaves only 3 of 19 passing. At 15:59:58 they report 29 Dino recordings and 63,000 frames, illustrating 1,800 steps, 23 obstacles and a pterodactyl before a crash, comparing positions, height, collision and score.

An existing secondary account at 18:17:04 on November 25 introduces GAME.md, input/random/state replay and Blocks without separate counts. The new candidate at 13:15:37 on November 26 adds six games and engine limits: externally replace the clock and Math.random, save a random-number tape, describe rules, per-frame ordering, constants and original bugs in GAME.md, then have a rebuilt program read cases on stdin and output a trace and tapeUsed for stepwise comparison.

Supplementary reading pins the README to 4480ef0474b65c0fadebbab89245ea1eb31682c5, committed at 01:01:12 Beijing time on November 26, before this window. It is project documentation, not another candidate. It confirms six web ports: 2048 has 19 cases/24,044 inputs; Dino 29/63,000 frames; Canvas Bird 30/68,409 frames; Blocks 36/104,208 frames; Bricks 37/209,600 steps; Paddles 19/198,300 steps. Rust/Bevy and Godot checks are listed for the first four; Bricks and Paddles are web-only. Canvas Bird's state is private, so an illustrated comparison uses draw calls instead, matching 1,140 steps. Docs say intentional collision, timing-gate or constant changes were rejected: changing Canvas Bird's 30 fps gate leaves 5/30 cases passing, alongside the 2048 odds mutation above.

Engine status needs qualification: Dino's Rust logic is checked through dino-runner, while the Bevy window reportedly only compiled and ran 25 seconds under Xvfb, never played. The playable Godot scene has only headless loading/input smoke checks and no visual inspection; an overview's 19-case phrase does not replace the per-game table. Unity and Capacitor are not started. Random consumption must match exactly, but only recorded behavior is checked, not every pixel or all possible inputs. Docs retain sparse flying-obstacle collision coverage in Dino and bottom-pipe collision coverage in Canvas Bird; network games and games with externally unobservable state need more work.

Public docs confirm Claude Code/Codex plugins and the study/spec/rebuild/check workflow. Implementation, raw recordings and the harness were not reviewed or run. All passes and figures remain project reports, not independent reruns. README family links to REA do not establish actual morluto/rea calls, so rea stays unknown and status unverified. Clean-room is the project's wording, not legal certification. No dependencies were installed and no game built or run.

Sealed root post: 0 likes, 1 view, 0 reposts, 1 reply. Engagement does not establish result credibility; reply figures were not independently rerun.
November 25, 18:17 secondary account: 38 likes, 746 views, 4 reposts, 2 replies in the sealed snapshot; not independent validation.
New November 26 candidate: 0 likes, 49 views, 0 reposts, 0 replies. Its 236-star/one-day-growth statement is secondhand; GitHub history was not checked.

## Sources

- [erKam introduces rea-games and cross-engine recorded comparisons, November 25, 2026 at 15:59:03 Beijing time](https://x.com/i/status/2125499490606145735)
- [Supplementary author reply: 19 recorded 2048 games, 24,044 inputs and a probability-mutation negative control, November 25, 2026 at 15:59:41 Beijing time](https://x.com/i/status/2125499651566522513)
- [Supplementary author reply: 29 Chrome Dino recordings and 63,000 frames, November 25, 2026 at 15:59:58 Beijing time](https://x.com/i/status/2125499725050745291)
- [Secondary account: GAME.md, input/state replay and Blocks, November 25, 2026 at 18:17:04 Beijing time; not independent validation](https://x.com/i/status/2125534226636509548)
- [New secondary account: six games, random tapes and engine limits, November 26, 2026 at 13:15:37 Beijing time](https://x.com/i/status/2125820752574509432)
- [Supplementary pinned README, committed November 26, 2026 at 01:01:12 Beijing time; pre-window docs, read but not rerun](https://github.com/erkamyaman/rea-games/blob/4480ef0474b65c0fadebbab89245ea1eb31682c5/README.md)

[中文](../rea-games-claude-cross-engine-recorded-behavior-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
