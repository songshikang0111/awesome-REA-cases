# Coway purifier off-cloud: a secondary account of HTTP root certificates and AI-assisted Bluetooth setup

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-14
Stage: Needs verification

At 01:32:44 Beijing time on November 14, 2026, a post relays off-cloud research on a Coway IoCare air purifier, motivated by official-cloud outages, app rewrites and account bans. It says setup downloads Amazon's root CA over plain HTTP. The owner reportedly isolates the device with a Raspberry Pi, observes traffic with mitmproxy and substitutes a trust root so the device accepts a different MQTT endpoint and Home Assistant can communicate directly. MQTT is a device-messaging protocol. This is an account of recovering local interoperability for an owned device, not a vulnerability discovered by this collection.

The post also says Bluetooth setup sends Wi-Fi credentials and cloud configuration in encrypted protobuf, and an AI combined Android logs and decompiled app code into a protocol in about 20 minutes. It supplies no model, tools, device model, firmware, logs, source or direct original-author link. Twenty minutes is a secondary claim, not the duration of the entire off-cloud project. No evidence establishes that every Coway model or current version accepts the substituted root, or independently validates Home Assistant stability or security. Identity with the existing Ryan Blass unnamed-purifier agent-swarm study cannot be established, so they are not forced into one record. No credentials were accessed, targets downloaded, devices connected or configurations executed here. REA use is unconfirmed; included as a low-detail, unverified secondary account of a concrete project.

Candidate snapshot: 2 likes, 83 views, 0 reposts, 2 replies. Twenty minutes is a secondary claim without reviewable logs.

## Sources

- [Secondary Coway/IoCare off-cloud and AI Bluetooth account, November 14, 2026 at 01:32:44 Beijing time](https://x.com/i/status/2121295210550571018)

[中文](../coway-iocare-ai-bluetooth-local-mqtt-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
