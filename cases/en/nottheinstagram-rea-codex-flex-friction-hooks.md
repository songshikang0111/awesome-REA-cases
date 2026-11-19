# NotTheInstagram: FLEX guides Codex with REA to slow endless scrolling

Category: Applications and clients · REA
Record date: 2026-11-20
Stage: Needs verification

At 01:01 Beijing time on November 20, 2026, lifcc (@mylifcc) introduces NotTheInstagram with article and repository leads. Kunal Kamble's November 15 original and project docs were read as supplementary evidence predating the strict window, not new candidates. He wants to keep friends' DMs, search and other useful Instagram features while adding friction to endless scrolling, rather than deleting the app.

The author uses Codex with REA connecting it to Hopper to investigate an approximately 400 MB executable. Initially the agent guesses class names and cannot find the Explore grid. The human inspects the screen's view tree with FLEX and supplies class names and screenshots, helping locate IGExploreGridViewController's viewWillLayoutSubviews and write Objective-C hooks. AGENTS.md records collaboration constraints and agents/ stores research and test status. The decisive map in the original is the FLEX view tree, not the retelling's claim of a complete architecture written after one runtime dump. Meta shared storage becoming inaccessible after re-signing also causes login failures and crashes; the author reports an adapter fix.

Reported behavior: each three feed posts wait 8, 11 and 14 seconds, then remain at 14; Reels waits two minutes at entry; each reel waits three seconds plus half a second per subsequent reel; DM reels do not advance into others; a label shows usage time. Most work reportedly took one afternoon, not a measured duration for the entire project. The README names Instagram 455.0.0, iPhone 15 and iOS 27.0.1 as its test environment.

Static reading of the README, RuntimeHooks.h and Explore notes at November 15 commit 206eac2 shows return-type, argument-count and argument-type checks before replacement. Notes explicitly distinguish static metadata from execution traces and leave individual search, rotation and accessibility checks unconfirmed. Hidden grids may still fetch data. No build, IPA acquisition or device reproduction was performed here. Compatibility across every update is not guaranteed; legally obtained targets are required and modified clients carry platform-rule and account risks. Status remains unverified.

Sealed candidate: 3 likes, 628 views, 0 reposts, 1 reply; source reply: 0 likes, 171 views. Not total project reach.

## Sources

- [lifcc introduces NotTheInstagram, November 20, 2026](https://x.com/i/status/2123461551197720607)
- [Same-thread article and source leads](https://x.com/i/status/2123461552271446033)
- [Supplement: Kunal's original, published November 15, 2026](https://rationalkunal.in/writing/make-instagram-boring-with-an-ai-agent/)
- [Supplement: README pinned to November 15 commit](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/README.md)
- [Supplement: method-signature checking implementation, static reading](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/NotTheInstagramFrameworkCode/NotTheInstagramFrameworkCode/Runtime/RuntimeHooks.h)
- [Supplement: Explore notes and pending device checks](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/agents/search-investigation/explore-grid-notes.md)

[中文](../nottheinstagram-rea-codex-flex-friction-hooks.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
