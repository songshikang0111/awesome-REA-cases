# Wear OS-style UI on an ESP32-S3 round display: PopaSpinka's Claude driver and sample-port report

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-22
Stage: Needs verification

At 02:16:34 Beijing time on November 22, 2026, RetroChainer retells YouTube creator PopaSpinka's project on a $40 Waveshare ESP32-S3 with a round 466×466 AMOLED display and no GPU. Factory icons reportedly tear while scrolling and cannot be finger-dragged. The post says the developer bypasses LVGL and Arduino_GFX, uses Claude Code to write display/touch drivers and a drawing library from scratch, then has Opus 5.5 port Google's open Wear OS samples: rolling digits, a Pixel Watch-style card gallery, weather and music interfaces.

Two days/two evenings, 60 FPS, zero dropped frames, no tearing and no draws at idle are secondary claims. The listed video positions, 3:22 for factory tearing and 4:16 for standard-driver flashing, were not watched or measured. This modifies existing open samples and device behavior; it does not break into a Pixel Watch or reproduce all technology Google acquired for $40.

A supplementary reader asks about the first frame after waking on battery, without a returned test answer. Reduced drawing is not measured battery life. No repository, code or flashing record was obtained; open-source availability and Chrome flashing also remain post claims. No target or dependencies were run. REA is unmentioned and status is unverified; Fable 5.2 is the poster's speculation, not a model used in the reported work.

Sealed candidate: 25 likes, 882 views, 2 reposts, 4 replies. This is not performance or battery validation.

## Sources

- [RetroChainer retells PopaSpinka's round-display drivers and Wear OS samples, November 22, 2026 at 02:16:34 Beijing time](https://x.com/i/status/2124205345606103149)

[中文](../popaspinka-esp32s3-wearos-ui-claude-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
