# HookLab: REA studies Creator Hooks; Claude rebuilds YouTube titles and an outlier library

Category: Applications and clients · REA
Record date: 2026-11-03
Stage: In progress

At 00:29 Beijing time on November 3, 2026, Samin Yasar (@SaminXD) reports canceling a $360/year YouTube tool and rebuilding it as HookLab with REA and AI coding agents. For video creators, it generates angle-grouped titles modeled on real outliers, searches videos outperforming their channel average, polls uploads and tags them with Claude, and exposes a CLI and REST API. The subscription price and cancellation are the author's account, not net operating costs.

This review read the public Samin12/hooklab README, HOW-IT-WAS-BUILT and app/package.json pinned to 1e5fcb584c98b0b3bfe44438ee4410414b91990d. That commit is dated October 19 at 06:00:22 Beijing time, before the candidate window: existing implementation/method background, not a new November 3 commit. The method names Creator Hooks as the reference: the author signed in using a dedicated browser profile, then used REA over DevTools to read DOM, accessibility trees, network metadata, storage keys and loaded scripts. Clicking through screens loaded lazy code before export. Minified bundles, 48 click-trigger labels and the absence of source maps informed the study; one real title-generation exchange captured requests and streamed responses. Claude Code built a foundation, four workers handled separate UI areas, and a data CLI/API and polling pipeline were added.

The notes claim My Channel's personal-video/recent-average multipliers reproduced the original values for every compared video. No sample count, original outputs or complete functional differential record is provided: neither server-side algorithm recovery nor full equivalence is established. The project says it contains no original code, assets or data; this collection did not audit that claim or clean-room isolation.

The README requires Node.js 24, Next.js 16 and local SQLite. A fresh library is empty and needs user-added channels. Chat/tagging require the Anthropic API or a signed-in Claude Code CLI; polling uses YouTube RSS, with optional ScrapeCreators for discovery and some metadata. Self-hosting does not mean offline or cost-free operation. Thumbnail search uses title text, not image embeddings; billing is a local credit ledger that charges nothing. Only public documents and the manifest were read: no dependencies, targets, authenticated services or comparisons were run here.

Candidate snapshot: 20 likes, 826 views, 2 reposts. $360/year is the author's former subscription cost, not evidence that AI and data services are free.

## Sources

- [Samin Yasar's HookLab/REA report, November 3, 2026](https://x.com/i/status/2117292948488400976)
- [Supplementary pinned README: existing implementation and dependencies, October 19, 2026, before the window](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/README.md)
- [Supplementary pinned method: Creator Hooks research and rebuilding, before the window](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/docs/HOW-IT-WAS-BUILT.md)
- [Supplementary pinned app/package.json: declared dependencies, not installed](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/app/package.json)

[中文](../hooklab-rea-youtube-outlier-tool-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
