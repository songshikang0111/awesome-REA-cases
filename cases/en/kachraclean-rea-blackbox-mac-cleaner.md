# KachraClean: REA black-box study of CleanMyMac informs developer and model-cache cleanup

Category: Applications and clients · REA
Record date: 2026-11-03
Stage: In progress

At 12:34 Beijing time on November 3, 2026, Nikhil Deshpande (@nikhdesh) introduces KachraClean 0.1.5: a commercial cleaner offered 17.6 GB while projects and models occupied much more. He reports 43.9 GB in 120 dependency/build folders and another 70.9 GB in model caches. These are candidate sizes on one Mac, not space already freed or proof that all the data is disposable.

Supplementary public documentation is pinned to 940a2f656d5fa82d8c30c66774ec1555e75cf17c, committed November 1 at 14:12 Beijing time. Its README and October 17–November 1 log predate this window and support the new report rather than count as new experiments. The log identifies CleanMyMac 5.7.2, REA 6.5.0 and Claude Code. The author sets rules against decompiling code or decrypting its rule database, studying bundle metadata, UI and behavior before writing independent specs. The 1,343,066 events were user-recorded with fs_usage and separately parsed with Python, not automatically captured by REA. REA's UI helper exceeded a 60-second cold-compilation timeout; the author compiled the same helper for reading, with the human clicking and the agent observing. Clean-room is the project's own process, not this collection's legal certification.

The log reports an approximately 2.5-minute reference scan using 107 threads; one observation without the privileged helper cannot cover all modules. Later, Spotlight metadata suggested the unused-app rule: the author predicted four apps before viewing the filter and reports all four matched. The implementation provides a Swift core, CLI and SwiftUI app: read-only scanning, per-item safe/review/risky labels with reasons, Trash removal and in-memory Undo. Undo is not persistent and cannot be relied on after restart or a crash; the log records a cleanup crash losing in-memory Undo, reportedly fixed in 0.1.4.

The November 1 security record admits that older saved reports could forge model findings to move arbitrary user files with Full Disk Access, and that docker executables in writable locations were launched. Version 0.1.5 reportedly adds per-category clean-time checks, no preselection of old reports, and a signature-restricted Docker CLI; tests grew from 38 to 46. These are project fixes and self-tests, not rerun here. Docker was tested against recorded output, not live hardware. The README's roughly 78 GB gap and the launch post's later breakdown must not be combined as one measurement. The app requires macOS 14+, has no paid Apple Developer account, is ad-hoc signed and not notarized. No app was downloaded, cleanup executed, or safety or equivalence independently verified.

November 3 candidate snapshot: 1 like, 129 views, 0 reposts. The 17.6/43.9/70.9 GB figures and 46 tests are author/project reports, not reproduced by this collection.

## Sources

- [Nikhil introduces KachraClean and its REA black-box study, November 3, 2026](https://x.com/i/status/2117475470036148719)
- [Supplementary README pinned to a November 1, 2026 commit, before the window](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/README.md)
- [Supplementary research/security log, October 17–November 1, 2026, pinned commit](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/case-study/log.md)
- [Supplementary scan-behavior spec: one observation without the privileged helper](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/spec/01-scan-behavior.md)
- [Supplementary cleanup-category spec retaining untested-module limits](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/spec/02-cleanup-categories.md)

[中文](../kachraclean-rea-blackbox-mac-cleaner.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
