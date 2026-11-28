# bouncemarket ball prediction: a Claude bot reports correct calls on 146 of 181 rounds, not advance knowledge of every round

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-28
Stage: Needs verification

At 14:23:49 Beijing time on November 28, 2026, AI Dev Daily (@AIDevDaily) describes bouncemarket, where players trade predictions of whether a bouncing ball lands left or right. It claims someone used Claude to reverse-engineer the physics engine with 146 correct calls, while another collected more than 600 rounds to investigate randomness. Supplementary reading of the original Hacker News discussion narrows these claims. Those comments are not additional current-window candidates.

In the Show HN introduction at 23:01:50 Beijing time on November 27, creator mday404 says the server simulates the drop in advance and streams coordinates through SSE. A trajectory is deterministic given its initial conditions. Built-in AI traders use the creator's simple handwritten rules and withdraw when more than five humans participate; they are not the player-built Claude bots. The creator later says clients receive coordinates rounded to 0.1px while simulation uses 64-bit floats, limiting early trajectory recovery.

At 03:47:48 on November 28, e1ghtSpace reports a bot built with Claude: 146/146 correct calls, but only 146 of 181 rounds called, skipping rounds it could not calculate in time. Reported profit of +98.80 is an in-game result, not verified cash earnings. Markets often already reached 0.99 when prediction became possible; 100% does not mean knowing every round at its start. Seed recovery was a proposed next version, explicitly of uncertain feasibility. At 06:42:15, SecuredMarvin reports Opus recovering floating-point starting positions and a plan to collect 600 rounds to solve the Mersenne Twister, interrupted by a server restart and deployments changing the conditions. This is not evidence that randomness was cracked. At 06:50:18, mday404 denies changing the RNG because of that post; the difference in attribution must remain visible.

The public discussion was read, but bot code, complete round logs and an executed reproduction were not obtained. The secondary post's 300-plus players, under eight hours and 0.1 seconds are not independent measurements or a basis for generalized profitability. No game connection or trade was made here. REA is unmentioned.

November 28, 2026 sealed candidate: 0 likes, 12 views, 0 reposts, 0 replies. The 146/181 result is a player's report, not an independent reproduction.

## Sources

- [Window candidate: AI Dev Daily's bouncemarket account, November 28, 2026 at 14:23:49 Beijing time](https://x.com/i/status/2126562690902774008)
- [Pre-window Show HN: mday404 on server-side physics simulation, November 27, 2026 at 23:01:50 Beijing time](https://news.ycombinator.com/item?id=50667726)
- [Pre-window e1ghtSpace: 146/181 round selection and skipped rounds, November 28, 2026 at 03:47:48 Beijing time](https://news.ycombinator.com/item?id=50670903)
- [Pre-window SecuredMarvin: 600-round RNG research interrupted by deployments, November 28, 2026 at 06:42:15 Beijing time](https://news.ycombinator.com/item?id=50672416)
- [Pre-window mday404: correction about why the RNG was not changed, November 28, 2026 at 06:50:18 Beijing time](https://news.ycombinator.com/item?id=50672463)

[中文](../bouncemarket-claude-physics-prediction-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
