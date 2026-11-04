# CS2 audio delay: Claude finds a 23ms parameter, but Thour retracts the hardware-confounded conclusion

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-04
Stage: Analysis test

At 12:40:36 Beijing time on November 4, 2026, Thour (@ThourCS2) publicly corrects his automatic-rifle audio-delay comparison between CS:GO and Counter-Strike 2. He says wired Sony speakers initially showed differences up to 20ms, whereas retesting on a Razer Blackshark V3 Pro headset, described as wired in his test, made the difference almost negligible. He apologizes for failing to control hardware variables and says @iamcs2kitchen's earlier analysis was correct.

He credits Claude with reverse-engineering game files to find snd_delay_sound_ms_shift defaulting to 23, but acknowledges that this 23ms parameter has not established the claimed general audio delay. His new tests report no AK-47 difference between the games; setting the parameter to 0 was 7.9ms faster than CS2's default 23. For M4A4, CS2 was reportedly 4.6ms slower than CS:GO and changing the parameter had no clear effect. The post's English wording about the M4A4 effect is imprecise; context supports a conservative reading of no clear improvement, not statistical significance or inferred measurement error.

This is an AI-assisted analysis report with a concrete negative result and correction, not a confirmed 23ms latency bug or optimization recommendation. No game revision, sampling method, repetition count, raw audio, Claude conversation or decompilation output is supplied. The author's suggestion that better hardware eliminates differences is also not a conclusion for all devices. The attached chart was not inspected and the games were not retested here. REA is not mentioned.

Sealed candidate snapshot: 158 likes, 8,253 views, 4 reposts; retained rather than replaced by changing retrieval metrics. The values 23, 7.9ms and 4.6ms are author reports.

## Sources

- [Thour's audio-delay correction and attribution of parameter research to Claude, November 4, 2026 at 12:40:36 Beijing time](https://x.com/i/status/2117839404903571758)

[中文](../cs2-claude-sound-delay-hardware-correction.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
