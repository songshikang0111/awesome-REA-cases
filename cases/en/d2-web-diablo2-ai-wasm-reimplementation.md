# D2-Web: human-directed AI assistance for a browser Diablo II 1.13c engine, still early Act 1 alpha

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-01
Stage: In progress

At 08:25:54 Beijing time on November 1, 2026, the candidate reports Virtastic's D2-Web, a C++20 reimplementation of the Diablo II: Lord of Destruction 1.13c engine compiled to WebAssembly. It executes locally in Chrome/Chromium rather than streaming a remote game. The post lists widescreen, controller input, seven classes, shared stash and autosaves, while explicitly calling it early Act 1 alpha, not the complete Diablo II.

Supplementary reading inspected README at 2bb0efe4808065b6a7d6409300da847c6757ec91, dated November 1 at 03:14:36 UTC, or 11:14:36 Beijing time, later than the candidate and used as primary-source context. It confirms heavy AI-tool assistance with human direction/review, study of the retail 1.13c program and a process that was not clean-room. Some code adapts MIT-licensed D2MOO and builds on StormLib and other prior work. The README specifically reports Act 1 character creation, camp, initial wilderness areas, combat, items, vendors, waypoints and saves, with missing screens and wrong behavior remaining. The candidate's seven-class and other feature claims were not tested individually.

Default BYO mode lets players select local MPQs that remain in the browser, but the documentation also supports server-hosted MPQs. Not every deployment can be described as keeping files unuploaded. The development server has no authentication; the README warns that anyone who can reach it can download configured MPQs, which must not be publicly redistributed. Wasm threads also require cross-origin isolation headers and HTTPS or localhost. Saves remain in each device's browser and Battle.net is disabled. MIT licensing for its own source does not permit redistribution of Blizzard assets; legally obtained 1.13c game files are required. Only documentation was read here, without dependency installation, game-data acquisition, server deployment or rerunning differential/game tests.

Candidate snapshot: 17 likes, 1,019 views, 1 repost. No independent gameplay or differential testing.
Supplementary documents postdate the candidate. BYO and hosted-file deployments have different privacy boundaries; early alpha is not a complete game.

## Sources

- [Candidate: D2-Web browser reimplementation and AI report, November 1, 2026](https://x.com/i/status/2116688145823486161)
- [Supplementary pinned November 1, 11:14 README: AI attribution, alpha and deployment boundaries](https://github.com/Virtastic/d2-web/blob/2bb0efe4808065b6a7d6409300da847c6757ec91/README.md)

[中文](../d2-web-diablo2-ai-wasm-reimplementation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
