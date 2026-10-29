# scapectl: Claude Code helps recover Fractal Scape USB HID and build a cross-platform controller

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-10-29
Stage: In progress

At 22:14:21 Beijing time on October 29, 2026, Jamie Dubs (@jamiew) introduces scapectl, an unofficial configurator for the Fractal Design Scape wireless gaming headset, crediting AI reverse engineering and repeated testing. His parent post announces v0.0.17 menu-bar state, boom-microphone events, improved receiver connection handling and once-per-episode low-battery notifications. Supplementary reading obtained the charlietran/scapectl README at commit 945ee25cda7487516a1ee0d02b436bff1923e457, timestamped 14:06:03Z that day, before the post. It explicitly credits Claude Code with understanding USB and implementing the cross-platform Go app. REA is not mentioned.

Research uses WebHID captures from Adjust Pro and its Electron app source, not AI guessing the protocol from scratch. Public documentation distinguishes receiver commands from headset relays and describes polling, EQ and microphone controls. It identifies an unreliable receiver presence field and microphone booleans whose source labels contradict hardware behavior, requiring device-based corrections. The app exposes battery/microphone status, EQ preset selection, RGB/noise-cancellation switches and events that invoke external scripts. Switching audio output still requires separate tools.

The README reports testing only on macOS and Windows; Linux is a build target, not established hardware validation. Bluetooth connection detection, full lighting themes, button customization and EQ import/export remain planned. Adjust Pro cannot share the same HID stream concurrently. The macOS app is not notarized and Windows binaries are unsigned. The project declares GPLv3 and credits dependencies. This collection only read documentation: it did not install the app, disable protections, connect a headset or retest the protocol. Status remains in progress.

Candidate snapshot: 0 likes, 30 views, 0 reposts. Parent post and repository are same-day supplementary evidence.
Public protocol and implementation do not constitute independent device tests. Linux is untested; macOS is not notarized and Windows is unsigned.

## Sources

- [Jamie Dubs credits AI reversing and testing for scapectl, October 29, 2026](https://x.com/i/status/2115809467967180976)
- [Supplementary: same author's v0.0.17 parent announcement, October 29, 2026](https://x.com/i/status/2115809465224294886)
- [Supplementary: pinned scapectl README, protocol reference and platform limits, October 29 commit](https://github.com/charlietran/scapectl/blob/945ee25cda7487516a1ee0d02b436bff1923e457/README.md)

[中文](../scapectl-fractal-scape-claude-usb-hid.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
