# Project Avalanche: Claude-assisted SSX 2012 disc and behavior research rebuilt in Rust/Bevy

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-09
Stage: In progress

At 06:34:13 Beijing time on November 9, 2026, The Gaming Emporium (@McGroin83) introduces MnkyArts' Project Avalanche: bringing EA's Xbox 360 snowboarding game SSX (2012) to modern PCs by researching disc data and game behavior and independently reimplementing them in Rust and Bevy, rather than Xbox 360 emulation or static recompilation. Supplementary review pinned the public README to 208af62913ea8b8f3f32a9530123783516aa83cc, committed November 9 at 00:14:15 Beijing time, and confirmed that its text matches the version read. This record predates the candidate and falls outside the current window; it is supplementary evidence, not another candidate post.

The project explicitly credits Claude-assisted development, formats studied from the maintainer's own retail disc and behavior read from game code. Credits list Ghidra exposed to tools through GhidraMCP, plus ImHex and Kaitai Struct for structural analysis; REA use is not claimed. Documentation describes boot movies, menus, new profiles, World Tour/Explore, rider physics, HUD, music, speech, effects, results and saved progress in one window. The launcher extracts approximately 4.7 GB from the user's own Xbox 360 ISO. Windows/Linux builds, dedicated servers, public listing and LAN discovery, Luau scripts, maps and gamemode mods are documented. These are project descriptions, not runs by this collection. The updater reportedly preserves saves and data; that is not a guarantee of risk-free upgrades.

The project reports retail-disc checks wherever possible, including whole-disc parser validation and comparisons against game code and reference decoders. Nevertheless, nobody has completed a full playthrough. Undecoded behavior is marked TODO(guess), with the address or open question that could resolve each approximation. Build and CI commands are documentation, not execution logs obtained here. End-to-end playability, equivalent original physics, stable networking and universal compatibility are not established. Linux documentation requires Vulkan, ALSA and Wayland/X11; builds target Ubuntu 24.04 x86-64 and its glibc or newer, not every Linux system.

Original project code is marked MIT, while SSX and its disc contents remain EA's property. The project says its repository and builds contain no game data; users need a legally obtained compatible retail-disc image. This collection read the post, public metadata and pinned README only. No release, game asset or target code was downloaded or executed, and no build or playtest was performed. Project-reported checks are not independent reproduction.

Sealed candidate: 4 likes, 327 views, 1 repost. Views changed on retrieval; sealed values are retained. Approximately 4.7 GB describes extracted game data, not reconstructed source size or correctness.

## Sources

- [The Gaming Emporium introduces Project Avalanche, November 9, 2026 at 06:34:13 Beijing time](https://x.com/i/status/2119559143551799341)
- [Supplementary project README pinned to the November 9, 2026 00:14:15 Beijing-time commit, with AI attribution and no-full-playthrough limit](https://github.com/MnkyArts/ProjectAvalanche/blob/208af62913ea8b8f3f32a9530123783516aa83cc/README.md)

[中文](../project-avalanche-ssx2012-claude-bevy-reimplementation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
