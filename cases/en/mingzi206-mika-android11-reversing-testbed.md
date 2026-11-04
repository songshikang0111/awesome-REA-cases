# A Mika phone-research testbed: Android 11 combines agent vision, root and traffic inspection

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-05
Stage: In progress

At 01:30:54 Beijing time on November 5, 2026, Mingzi206 (@mingzi206) reports spending another two days turning a real Android 11 phone into an agent-control testbed, connecting customized Mika to root and a traffic-inspection/reversing environment. Combining visual interaction with direct state reads aims to reduce slow, inaccurate screenshot/accessibility-only tapping.

The author reports taps, swipes, multi-app wakeups and automatic battery/network checks working, with phone_sense reading battery, temperature, Wi-Fi and notifications within seconds. Runtime permissions such as the Huawei browser microphone can reportedly be switched silently, AppOps changes reset after tests, and package-based SQLite queries pass on a self-created WAL database using single read-only snapshots to avoid concurrent locks. The reported research environment includes repairing /debug_ramdisk/su, restoring Magisk modules, Frida Server/getpid hooks, a dual-architecture LSPosed Binder bridge, system-trusted root certificates, positive/negative mitmproxy HTTPS checks and deployment SHA-256 comparisons. These are environment claims, not a general privilege-escalation method or certification for arbitrary apps.

The author claims 51 targeted unit tests and ten HTTPS assertions passed, while shared-screen actions still occupy the visible screen and newer GSI boot support remains in development. Device model, Mika source, model, assertions and checkable logs are absent. Tests do not establish coverage of every permission or actual app data, and the self-created database is not evidence of decrypting others' databases. No adb, injection, traffic capture, credentials or phone access was performed here. REA is not mentioned.

Sealed snapshot: 4 likes, 646 views, 0 reposts. Two days, 51 unit tests and ten HTTPS assertions are author figures; the video and tests were not rerun.

## Sources

- [Mingzi206's Android 11/Mika dual-mode research-testbed account, November 5, 2026](https://x.com/i/status/2118033257925365941)

[中文](../mingzi206-mika-android11-reversing-testbed.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
