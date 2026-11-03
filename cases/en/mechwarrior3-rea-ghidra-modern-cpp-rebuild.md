# MechWarrior 3: a modern C++ rebuild crediting REA and Ghidra

Category: Games and preservation · REA
Record date: 2026-11-04
Stage: In progress

At 02:51:07 Beijing time on November 4, 2026, a post introduces version 1.0 of Owen Morgan's MechWarrior 3 rebuild: native Windows, macOS and Linux support, widescreen and up to eight players for the 1999 PC mech game. Supplementary reading of the public README at commit bb9af7b22c54c909cec8052595c1fe0bb32773f1 explicitly credits Ghidra and REA for studying Mech3.exe 1.2 and rewriting it function by function in C++. The project cross-checks formats with mech3ax and compares against the original in Unicorn; it is not simply static recompilation or a Wine wrapper. The pinned commit is dated November 4 at 01:29:09 Beijing time and supplements the method/scope evidence rather than constituting another candidate.

The README describes SDL3 with Direct3D 12, Metal and Vulkan backends, loading 1.0 data with 1.2 behavior, and custom UDP networking replacing DirectPlay, alongside original mechanics and compatibility fixes. Users must supply their own game files; no game assets are distributed. Pirate's Moon is unsupported. The candidate explicitly says the Linux AppImage was built but not play-tested, so a three-platform release list is not three-platform testing. Reported emulator comparisons for most logic were not rerun here and establish neither full byte matching nor independently accepted campaign completion or cross-platform multiplayer. No release, dependencies or game were downloaded, built or run.

Candidate snapshot: 11 likes, 410 views, 1 repost. Linux play-testing and expansion support remain explicitly limited.

## Sources

- [Introduction to the modern MechWarrior 3 rebuild, November 4, 2026](https://x.com/i/status/2117691059149115770)
- [Pinned project README: REA/Ghidra credits, method and scope; commit dated November 4 Beijing time](https://github.com/telltaleatheist/mw3-re/blob/bb9af7b22c54c909cec8052595c1fe0bb32773f1/README.md)

[中文](../mechwarrior3-rea-ghidra-modern-cpp-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
