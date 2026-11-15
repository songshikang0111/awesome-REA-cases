# Coway Airmega IconS off-cloud: secondary accounts of HTTP root certificates, AI Bluetooth research and a Web Bluetooth installer

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-15
Stage: Needs verification

At 01:32:44 Beijing time on November 14, 2026, a post relays off-cloud research on a Coway IoCare air purifier, motivated by official-cloud outages, app rewrites and account bans. It says setup downloads Amazon's root CA over plain HTTP. The owner reportedly isolates the device with a Raspberry Pi, observes traffic with mitmproxy and substitutes a trust root so the device accepts a different MQTT endpoint and Home Assistant can communicate directly. MQTT is a device-messaging protocol. This is an account of recovering local interoperability for an owned device, not a vulnerability discovered by this collection.

The earlier post also says Bluetooth setup sends Wi-Fi credentials and cloud configuration in encrypted protobuf, and an AI combined Android logs and decompiled app code into a protocol in about 20 minutes. A secondary account at 09:00:02 on November 14 names Coway Airmega IconS, Android Bluetooth debug logs and an AI coding agent, saying the setup payload directly specifies certificate-server URLs. It also describes an open-source Chrome Web Bluetooth installer that pairs the purifier directly to local Home Assistant without soldering or the vendor cloud.

A new candidate at 14:01:00 on November 15 names the researcher as Scott Goldman. It specifically says AI collected Android Bluetooth HCI logs through adb and decompiled the official APK, reconstructed the encryption algorithm in about 20 minutes and found that the phone sends root-certificate and cloud-API addresses during setup. HCI logs record communication between the host and Bluetooth controller; these are reported research materials, not captures obtained here. The post again claims a Web Bluetooth script redirects the purifier to local Home Assistant and Apple Home without opening/flashing the device or using a router proxy. Its zero-latency wording has no measurements. The name and capture path add secondary attribution and method details, not independent hardware acceptance testing.

No direct original-author page, source repository, firmware version, debug logs or installer code was obtained. Open source and no soldering remain attributed claims; the AI model and exact agent are unspecified. Twenty minutes refers to the reported Bluetooth-protocol work, not the whole off-cloud project. Applicability to every Coway model or current firmware, Home Assistant stability, security and fully offline operation are not independently established. Identity with the existing Ryan Blass unnamed-purifier agent-swarm study cannot be established, so they are not forced into one record. No credentials were accessed, targets downloaded, devices connected or configurations executed here. REA use is unconfirmed; status remains an unverified secondary report.

November 14 earlier post snapshot: 2 likes, 83 views, 0 reposts, 2 replies. Twenty minutes is a secondary claim without reviewable logs.
November 14 at 09:00 candidate snapshot: 0 likes, 27 views, 0 reposts, 1 reply; not installer validation or model-compatibility statistics.
November 15 candidate snapshot: 3 likes, 668 views, 0 reposts, 2 replies. Zero latency is unmeasured and not retained as a performance figure.

## Sources

- [Secondary Coway/IoCare off-cloud and AI Bluetooth account, November 14, 2026 at 01:32:44 Beijing time](https://x.com/i/status/2121295210550571018)
- [Secondary account: Airmega IconS, certificate URLs and Web Bluetooth installer, November 14, 2026 at 09:00:02 Beijing time](https://x.com/i/status/2121407777146892459)
- [New secondary account: Scott Goldman attribution and adb/HCI capture path, November 15, 2026 at 14:01:00 Beijing time](https://x.com/i/status/2121845904730890524)

[中文](../coway-iocare-ai-bluetooth-local-mqtt-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
