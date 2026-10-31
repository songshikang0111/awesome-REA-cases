# Android security audit: Forem proposes Claude investigation through ADB and jadx

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-01
Stage: Needs verification

At 03:29:19 Beijing time on November 1, 2026, Forem (@0xForem) proposes connecting an owned or authorized Android phone to Claude Code through ADB for a read-only security audit. Steps cover package names, install dates/sources, hidden launcher icons and misleading system-like names; accessibility, device-admin, notification, microphone, location and overlay permissions; then screen-off battery use, seven-day traffic and nighttime uploads. Suspicious APKs would be extracted and analyzed with jadx for server addresses, gallery/screenshot/keystroke code and upload timers.

The requested report explains risks, visible data and destinations, install dates, and an evidence-first removal plan requiring human confirmation. The prompt does not itself establish maliciousness: permissions or names alone cannot prove spyware. Available traffic, timing and permission data vary by Android version/device state; seven-day history, precise nighttime uploads and original-source recovery are not guaranteed. No actual phone, sample, logs or execution results are provided. No device connection, APK extraction, code execution or removal occurred here. Retained as a concrete AI-assisted reverse-engineering investigation idea, with REA use unconfirmed.

Candidate snapshot: 0 likes, 35 views; prompt not executed and no malicious sample confirmed.

## Sources

- [Forem's ADB/Claude/jadx audit prompt, November 1, 2026](https://x.com/i/status/2116613505260646834)

[中文](../forem-android-adb-jadx-claude-audit-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
