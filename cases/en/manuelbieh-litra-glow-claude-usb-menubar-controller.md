# Litra Glow without G HUB: Manuel Bieh reports a roughly 2 MB Claude-assisted menu-bar controller

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-15
Stage: Needs verification

At 19:30:01 Beijing time on November 15, 2026, Manuel Bieh (@ManuelBieh) introduces a controller for his Logitech Litra Glow webcam light. Wanting simple switching and adjustment without an approximately 1 GB G HUB installation, he says he had Claude investigate the USB protocol and build a roughly 2 MB macOS menu-bar app. He recalls the lamp unexpectedly switching on and changing during development, and reports brightness, color-temperature and on/off controls with a right-click shortcut. This is the author's device experience, not a reproduction by this collection.

The post's short link resolves to manuelbieh/litra-glow-controller. Supplementary research read the README at 641005a63a97daeeea8637922672b75ca3f9af97, committed October 25, 2026 at 03:58:54 UTC, before this window, as project background only. It documents USB HID, brightness from 20 to 250 cd/m², color temperature from 2700 to 6500 K, optional launch at login and a bundled litra.py scripting tool. It requires macOS 13 or later and uses ad-hoc signing. These are documented control ranges, not optical measurements made here.

An important attribution distinction: the README explicitly uses a protocol reverse-engineered by the open-source community, so Claude is not credited with independently discovering every USB command from scratch. The README describes G HUB as over 500 MB, while the post says about 1 GB; these are different approximate source figures, not measured installation or runtime usage. The roughly 2 MB figure is also the author's statement. Claude Opus 5.5 co-authorship on the pinned commit supports attribution of that patch, not a complete model trace for protocol discovery. The project states MIT licensing and no Logitech affiliation. This collection downloaded no binaries, ran no scripts, installed no application and connected no lamp. REA is unmentioned; status remains unverified.

Sealed candidate: 1 like, 15 views, 0 reposts, 2 replies. No development duration given.
About 1 GB and about 2 MB are author approximations; the README separately calls G HUB over 500 MB. No controlled size or memory comparison.

## Sources

- [Manuel Bieh's Claude/USB and roughly 2 MB controller report, November 15, 2026 at 19:30:01 Beijing time](https://x.com/i/status/2121928704376885636)
- [Pre-window pinned README: controls, USB HID and community protocol attribution, committed October 25, 2026 at 03:58:54 UTC](https://github.com/manuelbieh/litra-glow-controller/blob/641005a63a97daeeea8637922672b75ca3f9af97/README.md)
- [Same pinned commit: Claude co-authorship and installation-path patch](https://github.com/manuelbieh/litra-glow-controller/commit/641005a63a97daeeea8637922672b75ca3f9af97)

[中文](../manuelbieh-litra-glow-claude-usb-menubar-controller.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
