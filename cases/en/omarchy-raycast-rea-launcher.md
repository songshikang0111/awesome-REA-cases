# oma-launcher / oma-cast: a REA-informed Raycast-style launcher with an author video

Category: Applications and clients · REA
Record date: 2026-10-31
Stage: In progress

At 03:34 Beijing time on October 20, @typecraft_dev reports building an Omarchy Raycast-style launcher with REA in a few hours: habit-based ranking, unified app/Omarchy-action search, aliases, favorites, keyboard controls and live themes, reportedly opening in about 40 ms. Earlier supplementary reading uses typecraft-dev/oma-cast commit 9375380fe04dc67fd06752d884ea8cfe9d1eabad (October 20, 03:20), still named oma-launcher. The later 04:03 rename is not backdated into that original window.

Reading covered its README, RootSearch.js and relevant visible portions of the backend research notes. It requires Omarchy 4, Hyprland 0.56+ and omarchy-shell, running as a QML plugin rather than Electron/Node daemons. Code shows app/menu candidates, aliases, favorites, frecency and search fallbacks. Notes identify Raycast 2.8.2, separate static observations from inferences and disclose a Hopper timeout opening a native module through REA; some constants were read with objdump instead. Not every finding can be attributed to REA.

Settings, Script Commands, clipboard history, snippets, quicklinks, calculator, Raycast extensions, window management and rayconfig import remain roadmap items in that pinned revision, not a complete Raycast replacement. Independent clean-room and no-Raycast-code/assets statements are project claims, not legal review. No AI features in the product does not imply no AI-assisted development. Unit and smoke test files exist, but the earlier Actions endpoint returned no runs and this collection ran no target tests or desktop session. A few hours, about 400 menu actions and 40 ms remain author/project claims.

At 23:35:10 Beijing time on October 31, 2026, the same typecraft author announces a video about REA and making omacast. Original-post lookup confirms the account; public link entities expand to YouTube uMoRUue2wzI, titled I used the viral reverse engineering tool. This adds a traceable author-demonstration entry point without counting the existing project twice. The video was not played and no transcript obtained. Its title establishes neither completed new features, passed differential tests nor completion of the old roadmap; pinned-code evidence retains its original date and scope.

October 20 candidate: 106 likes, 1,985 views, 3 reposts. Retrieval then: 130 likes, 2,458 views, 3 reposts, not performance validation.
October 31 video candidate: 16 likes, 1,208 views, 0 reposts. Video not watched and new features not validated.

## Sources

- [typecraft's REA launcher announcement](https://x.com/i/status/2112266105200800245)
- [Pinned in-window README and roadmap](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/README.md)
- [Same commit's RootSearch implementation](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/plugin/core/RootSearch.js)
- [Same commit's Raycast static research and Hopper timeout disclosure](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/reference/02-backend.md)
- [Author's REA/omacast video announcement, October 31, 2026](https://x.com/i/status/2116554581580886102)
- [Supplementary author video link: I used the viral reverse engineering tool; not watched](https://www.youtube.com/watch?v=uMoRUue2wzI)

[中文](../omarchy-raycast-rea-launcher.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
