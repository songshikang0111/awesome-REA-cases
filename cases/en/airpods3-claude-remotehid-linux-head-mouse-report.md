# MousePods: Claude-assisted RemoteHID research turns AirPods into a Linux mouse and game head tracker

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: Needs verification

A Chinese retrospective at 21:17:00 Beijing time on November 5, 2026 describes Claude Code helping AirPods 3 become a Linux head-controlled mouse. After roughly 300 failed blind probes, research shifted to Wireshark, clone-earbud disassembly and iOS framework pseudocode. At 09:01:26 on November 11, Darrel Ang (@darrelang) names MousePods, AirPods 3/Pro 2 and no firmware changes. At 09:22:59, Dopax (@tensorstaff) adds RemoteHID/AACP docs, no intervening Apple device and 400-plus tests. Both new candidates supplement the existing target, not three independent validations.

This review finally located public starman-tech/mousepods, pinning commit 310c79b1751b6b590e5899e518d67026c76138d9, dated November 10 at 23:53:15 Beijing time, before this window. This is supplementary project documentation, not a new release in this window. README identifies Matteo Gaudioso, who says he reverse-engineered it with Claude as a pair engineer: Claude handled probes, cross-project static research, controller and tests, while the human held the earbuds, made decisions and checked hardware. One afternoon is the author's account; AI sessions and independent hardware experiments were not obtained here.

README and DISCOVERIES explain that AirPods 3 use RTBuddy's RemoteHID virtual-HID path, while Pro 2 use SensorDataWX. AACP/L2CAP data becomes head orientation and uinput cursor control on Wayland/X11 without flashing earbud firmware. The project marks AirPods 3 and Pro 2 hardware-verified; the original findings name AirPods 3, marketing firmware 6296592, Ubuntu 24.04, BlueZ 5.72 and Python 3.12. It says larger sensor descriptors are invisible at MTU 672 and appear at 2582, but explicitly retains a confound: Apple PnP DeviceID and re-pairing also changed before first success. Whether MTU alone suffices remains unisolated, not a completed single-variable causal experiment.

Project measurements range from 25Hz to roughly 210Hz, with twelve gaps over 50ms in 23 seconds at roughly 180Hz, motivating a 100Hz default. This refines the older approximately 200Hz retelling; it is not stable 210Hz for all earbuds. Sensors turn off in the case, changing the primary bud cancels streams and stationary fused data can freeze. README lists Pro 2 head tracking in Assetto Corsa and ETS2 on Bazzite tested by contributor henningnorden. The Games page places TrackIR/FreeTrack DLLs in Proton prefixes, so this is not entirely modification-free for the host or games. Pointer calibration is simulation-tested only; glide, head/jaw gestures and some earbuds remain experimental. Windows/Android are unsupported; Linux does not imply every distribution is validated.

README now says 400-plus tests while the older DISCOVERIES reproduction section still says 37: documentation evolution, not counts or reruns by this collection. Static reading of test_mouse_off_by_default.py shows assertions for paused defaults, no cursor movement, persistent pause and restoration of existing game bridges. This establishes neither a passing full suite nor safety in arbitrary environments. The docs label code Apache-2.0 and findings/docs/captures CC BY 4.0 with attribution; optional garmin-ble is AGPL-3.0-only with additional bundling obligations. Garmin is not a candidate target and receives no new entry. First-public priority remains the project's claim within its November 4 search scope, not an independently checked historical first. REA is unmentioned. This collection installed nothing, ran no tool, connected no Bluetooth and changed no games; status remains independently unverified.

November 5 sealed snapshot: 11 likes, 1,297 views, 0 reposts, retained as the older report's snapshot.
November 11 candidates respectively: 0 likes/25 views/0 reposts and 0 likes/42 views/0 reposts. 358 stars is Dopax's dated text claim, not a measurement here.
Pinned commit: 2026-11-10T15:53:15Z. Hardware checks, approximately 210Hz and 400-plus tests are project reports, not reproduced here.

## Sources

- [Older Chinese Claude Code/RemoteHID/Linux MTU retrospective, November 5, 2026](https://x.com/i/status/2118331749214175491)
- [Darrel Ang adds MousePods identity, Pro 2 and no firmware modification, November 11, 2026 at 09:01:26 Beijing time](https://x.com/i/status/2120320966144270592)
- [Dopax adds RemoteHID/AACP and 400-plus tests, November 11, 2026 at 09:22:59 Beijing time](https://x.com/i/status/2120326389081559054)
- [Supplementary pinned README: author, Claude's role, support and licensing; November 10, 2026 commit](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/README.md)
- [Supplementary pinned DISCOVERIES: measurement environment, unisolated MTU and stream-drop limits](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/docs/DISCOVERIES.md)
- [Supplementary paused-default/game-bridge regression tests, read statically, not run](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/tests/test_mouse_off_by_default.py)

[中文](../airpods3-claude-remotehid-linux-head-mouse-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
