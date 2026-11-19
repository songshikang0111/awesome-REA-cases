# GTA VI police behavior: RazeDen reports Opus reading 50 HUD frames to infer pursuit rules

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-19
Stage: Analysis test

At 19:17:45 Beijing time on November 19, 2026, RazeDen (@razeden0) claims to analyze GTA VI police AI. On a Mac, PS5 Remote Play and ffmpeg extract one frame every two seconds from a 100-second chase; Claude Code with Opus 5.5 reads 50 HUD frames for wanted stars, minimap police dots and cash to produce a behavioral specification. The author reports fifteen minutes of setup and one evening of research. This is screen-behavior investigation, not access to Rockstar source or decompilation of police code. Its specific observation experiment is recorded separately from existing whole-game port and mechanics-reconstruction wishes.

Reported observations are two police dots at zero seconds and 31 at 64 seconds while stars rise from one to five; a twelve-second flashing-star period after breaking line of sight, losing a star if hidden throughout and resetting if seen at second eleven; and four of every six new dots appearing in front of the car at three stars. The author says five-star arrest costs $8,600 of $21,500 and one-star death $1,500, and explicitly flags an inconsistency: zero minimap cops at 74 seconds despite a visible cruiser. These are the author's readings and inferences for the described clip. Dots need not count every officer, and correlation in one clip does not establish universal spawning, visibility or timing rules.

The reported bill is about 1,600 tokens per frame for 50 frames, 80,000 image-input tokens plus 30,000 prompt-input and 25,000 output tokens, costing $0.94 total or about $0.019 per frame. Model pricing, token logs and billing were not verified. Comparing Rockstar's claimed roughly $2 billion and eight years with one observation's cost mixes scopes and is not adopted as a reversing-efficiency ratio; release date and budget are not verified. Original wording and attribution were retrieved, not the reference video, raw frames, full specification, session, repeated experiments or actual game revision. The footage's identification as GTA VI is unconfirmed. The author also acknowledges that the model reads gameplay rather than makes the game. Retained as an independently unreproduced analysis-test; no game download or target execution occurred here. REA is unmentioned.

Sealed candidate: 1 like, 268 views, 0 reposts, 0 replies. Fifty frames, twelve seconds and $0.94 are author reports, not measurements by this collection.

## Sources

- [RazeDen's frame-by-frame HUD police-behavior account, November 19, 2026 at 19:17:45 Beijing time](https://x.com/i/status/2123375169494282725)

[中文](../razeden-gta6-hud-opus-police-behavior-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
