# Soundcore D3200 to Mac dictation: an agent-assisted live-audio client adaptation idea

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-12
Stage: In progress

At 09:39:52 Beijing time on November 12, 2026, AI产品黄叔 (@PMbackttfuture) discusses using an Anker recorder instead of a Typeless-like dictation workflow. The author says they use WeChat dictation on a Mac and suggests slightly modifying tacshi/Soundcore with an agent, or building an ASR input method. The post simultaneously claims the problem solved with zero cost and latency and says the final step of pasting recognized text at the current cursor is missing. It is not presented as a delivered end-to-end input method.

Another candidate at 09:34:11 introduces Soundcore Manager, a Flutter local client for soundcore Work D3200 independent of Feishu. Supplementary README reading is pinned to tacshi/Soundcore commit bfd764a2aad55aca103a86e7d6ca2c814d3f7f9c, dated September 11, 2026 at 19:20 Beijing time, before this window, solely to check underlying capabilities. It lists Android/iOS/macOS, BLE pairing and live audio, recording management, SoftAP export and Apple on-device or Soniox transcription. Apple on-device support is qualified by iOS 26 and device/language availability; this does not establish the same interface on Mac. Soniox's batch path uploads recordings, so local management is not necessarily offline or free.

This is agent-assisted adaptation of an existing protocol client, not proof that AI reversed the upstream protocol. It shares D3200 hardware with baseline BeanScribe but has a different implementation and purpose: a Flutter client toward insertion at the Mac cursor, versus BeanScribe's Feishu H5/Python and document workflow. Their results are not merged. The author says the repository lacks a license; only the README, not the full license tree, was reviewed here. Their assertion that personal use is legally unproblematic is not endorsed. The attached video was not reviewed, and no adaptation commit, end-to-end test or latency measurement was obtained. Work remains in progress. This collection built nothing, connected no device and called no speech service.

Sealed main post: 13 likes, 1,293 views, 1 repost, 4 replies; feature-introduction post: 3 likes, 46 views, 0 reposts. The author claimed 237 stars that day; this was not independently checked. Zero cost and latency were not measured.

## Sources

- [AI产品黄叔's agent-adaptation and Mac-dictation proposal, November 12, 2026 at 09:39:52 Beijing time](https://x.com/i/status/2120693023420112940)
- [Same-window Soundcore Manager D3200 feature introduction, November 12, 2026 at 09:34:11 Beijing time](https://x.com/i/status/2120691593128640855)
- [Supplementary pinned README committed September 11, 2026 at 19:20 Beijing time, before the candidate; statically read November 12](https://github.com/tacshi/Soundcore/blob/bfd764a2aad55aca103a86e7d6ca2c814d3f7f9c/README.md)

[中文](../soundcore-d3200-agent-mac-dictation-adaptation-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
