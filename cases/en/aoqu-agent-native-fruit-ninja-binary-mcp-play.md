# Fruit Ninja binaries to MCP: Kimi K3 moves real-time slashing into auto_play in a three-round comparison

Category: Games and preservation · REA
Record date: 2026-11-26
Stage: Analysis test

At 03:01:26 Beijing time on November 26, 2026, Ao Qu (@ao_qu18465) introduces Agent-Native Computer Use with Fruit Ninja: an agent studies internal state from compiled software binaries and builds an MCP service tailored to itself rather than operating screen by screen. A new candidate at 11:31:04 relays the same study's FreeCAD and Fruit Ninja results. These are separate targets; CAD's 55× speed/35× token figures do not apply to the game. This review reads the pinned study body at c822a0c, already referenced by the FreeCAD entry, to fill in the game method and results. It is supplementary reading of existing public research, not a new experiment in this window.

The documentation says Kimi K3 receives only the game binary and REA, without source, documentation or network access, and builds an MCP server through research, runtime validation, server creation and call checking. It then plays three 60-second rounds with the server and three with screen-based computer use. REA-server final scores are 287, 328 and 299, averaging 304.7; computer use scores 74, 66 and 63, averaging 67.7; the server built without REA scores 115, 198 and 109, averaging 140.7. Totals include end bonuses and are not direct measures of fruit-slashing performance. Points in play are respectively 202/243/229, 9/6/3 and 40/137/93, summarized by the project as means of 225, 6 and 90.

The server's auto_play reads fruit and bomb positions/velocities from game memory and slashes many times per second. The model normally calls it only one to three times per round; this is not frame-by-frame or slash-by-slash LLM reasoning. Without REA, the server captures the screen at 30 frames per second, tracks fruit over at least three frames and simulates 200 ms mouse strokes. Documentation separates the gains from moving real-time decisions into a server and then replacing window observation with memory state. The appendix lists five tools: get_state, auto_play, slash, start_mode and restart_round.

These are project-reported methods, text and chart alternative text, read but not rerun here. Server source, complete raw logs, video and game revision/platform were not reviewed; there is no human comparison or generalization evaluation, so expert-level remains the author's characterization. Continuing to reshape tools during future tasks is a proposal, not demonstrated ongoing adaptation. No game was run, assets downloaded or dependencies installed. analysis-test is retained; pinned text explicitly identifies REA, replacing the earlier uncertain classification.

Original introduction shares a snapshot with FreeCAD: 22 likes, 1,227 views, 5 reposts, 6 replies; not two independent validations.
The 11:31 secondary candidate has 0 likes, 171 views, 0 reposts, 2 replies. Pinned methodology was read this review; tests were not run.

## Sources

- [Ao Qu's Agent-Native Computer Use and real-time Fruit Ninja claim, November 26, 2026 at 03:01:26 Beijing time](https://x.com/i/status/2125666188630073806)
- [Secondary account of FreeCAD and Fruit Ninja results, November 26, 2026 at 11:31:04 Beijing time](https://x.com/i/status/2125794440963035505)
- [Supplementary pinned study body: Fruit Ninja's three-round scores, ablation and auto_play; author research from November 26, 2026, not a new experiment in this review](https://github.com/MIT-MI/Agent-Native-Computer-Use/blob/c822a0c47cdea82fa28b3955a4216c80f1cc5db9/index.html)

[中文](../aoqu-agent-native-fruit-ninja-binary-mcp-play.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
