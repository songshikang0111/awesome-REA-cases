# Stopwatch Micro: unofficial Codex Micro-compatible firmware and a quota bridge for M5Stack StopWatch

Category: Hardware and interoperability · REA use unconfirmed
Record date: 2026-11-01
Stage: Needs verification

At 09:56:53 Beijing time on November 1, 2026, the author introduces Stopwatch Micro, firmware for the M5Stack StopWatch Dev Kit (ESP32-S3) claimed to make ChatGPT Desktop recognize it as a Codex Micro over Bluetooth HID. The aim is keyboard-free approval/rejection, new tasks, switching agent conversations and viewing quota. The post describes C++/LVGL under MIT, with Plan, Fast, Approve, Decline, New Task and Fork buttons, an arc touch area for reasoning effort, plus push-to-talk and send controls.

The author explicitly says quota is outside the Codex Micro protocol. A separate Windows bridge reads it from the Codex App Server bundled with ChatGPT Desktop and sends it to the watch over Bluetooth HID. No API key, no copied login token and USB-free operation are project claims, not credential or traffic audits. Data becomes stale after two minutes without refresh and unavailable after ten, rather than pretending to be fresh: a concrete freshness policy.

The post reports v0.4.0 hardware tests of 17/17 HAL checks, 13/13 controls and 151/151 transmissions at 50 Hz without loss, warning that desktop updates may require compatibility changes. Inspectable code, logs, pinned revision and protocol documents were not obtained. These self-tests are not independent reproduction or a guarantee across Desktop versions. AI involvement in firmware development and the particular reversing method are unspecified. Retained as an interoperability project for AI tools with unknown tooling, without guessing REA use. No flashing, desktop-client operation or access to login material occurred here.

Candidate snapshot: 2 likes, 86 views, 0 reposts. The 17/17, 13/13 and 151/151 figures are author self-tests; logs not inspected.

## Sources

- [Author's Stopwatch Micro v0.4.0 compatible-firmware report, November 1, 2026](https://x.com/i/status/2116711041413378459)

[中文](../stopwatch-micro-codex-hid-compatible-controller.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
