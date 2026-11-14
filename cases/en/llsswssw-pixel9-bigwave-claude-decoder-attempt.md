# Pixel 9 bigwave hardware decoding: Claude reportedly collects stock-decoder data through Waydroid, with initial runs but problems remaining

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-14
Stage: In progress

At 22:40:24 Beijing time on November 13, 2026, @llsswssw3243 says Claude started reversing Pixel 9's bigwave dedicated video decoder. The author emphasized legal ownership and cited community reversing of Mali GPU drivers, saying Claude agreed and continued. The bigwave name and decoder characterization follow the author, without independent establishment of chip internals or expansion into a complete GPU driver.

A new candidate from the same author at 20:43:29 on November 14 says bigwave hardware decoding now runs, while explicitly retaining numerous problems and a need for extensive testing. The added method is Claude capturing data from Android's stock decoder in a Waydroid environment. Waydroid provides an Android runtime, but the post supplies no capture tool, data type or execution location. Recovery of every register/protocol or support for every video format is not invented. This advances the earlier agreement-to-research stage to an initial runtime report, not stable usability or complete-driver acceptance.

The earlier post recalls refused Pixel 4 modem research, recorded separately; Mali is an analogy, not a third project. A pre-window November 1 post at 09:28:26 reports Pixel 9 mainline Linux, KDE external display at 1080p 120Hz and brightness control. That does not establish the same bigwave build or measured display/decoding performance. Public source, firmware revisions, test-clip/format lists, error logs, frame rates and output comparisons remain absent; the image was not interpreted. REA use is unconfirmed. No device material was obtained, target code executed or result reproduced here. The author report remains in progress.

November 13 candidate shared by two Pixel targets: 1 like, 107 views, 0 reposts, 0 replies. Engagement is not counted twice.
The November 1 background post at 09:28:26 Beijing time reports 1080p 120Hz and brightness control only as mainline Linux usage, not a bigwave decoding test.
November 14 sealed candidate: 0 likes, 43 views, 0 reposts, 0 replies. Runs and remaining problems are both author-reported, without reviewable test data.

## Sources

- [Candidate: Claude begins Pixel 9 bigwave research, November 13, 2026 at 22:40:24 Beijing time](https://x.com/i/status/2121251842911035860)
- [Out-of-window supplement: the author's Pixel 9 mainline Linux usage context, November 1, 2026 at 09:28:26 Beijing time; not decoder validation](https://x.com/i/status/2116703883460592035)
- [New progress: bigwave runs, Waydroid stock-data capture and further testing needed, November 14, 2026 at 20:43:29 Beijing time](https://x.com/i/status/2121584804378632356)

[中文](../llsswssw-pixel9-bigwave-claude-decoder-attempt.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
