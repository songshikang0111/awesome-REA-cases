# Omarchy on a 16-inch M5 Pro: Julian Arango credits Claude with installer and Wi-Fi fixes

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: In progress

At 07:20:59 Beijing time on November 23, 2026, Julian Arango (@ja818_) reports a weekend with Claude Code getting Omarchy running natively on a 16-inch M5 Pro MacBook Pro. He says omarchy-m5 documentation still excludes the 16-inch model, so he patched the installer to accept it. The unchanged 14-inch image reportedly boots with normal Apple 27.2 firmware, no macOS beta and all eighteen CPU cores. This is the author's adaptation report, not Apple specifications or complete driver support verified by this collection.

Wi-Fi reportedly did not initially appear because one device-tree line for the 16-inch model waited indefinitely for a power pin Linux does not yet set up on M5 Pro. Removing the line made Wi-Fi appear. The home router then reported a wrong password despite correct credentials; the author says he fixed the driver's refusal of WPA/WPA2 mixed mode and sent the change upstream. Keyboard, trackpad, Wi-Fi, Bluetooth, USB, lid sleep and battery reportedly work, while sound, GPU and camera are next. This concrete compatibility-debugging task is retained as broader AI-assisted hardware research, not a claim of recovering drivers from closed firmware or the same project as other authors' Mac or Shield ports.

Original-post retrieval confirms attribution and two photo attachments. Images, repository, patches, upstream acknowledgment, boot logs and stability tests were not reviewed. A weekend is retrospective effort, submission upstream does not mean a merge, and booting does not imply full hardware support. Status remains in-progress. No system was installed or project executed here; REA is unmentioned.

Sealed snapshot: 1 like, 23 views, 0 reposts, 1 reply. A weekend, eighteen cores and firmware 27.2 are author claims; patches and hardware were not checked.

## Sources

- [Julian Arango's 16-inch M5 Pro/Omarchy Claude Code adaptation report, November 23, 2026 at 07:20:59 Beijing time](https://x.com/i/status/2124644341129888078)

[中文](../julian-arango-16inch-m5-pro-omarchy-claude-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
