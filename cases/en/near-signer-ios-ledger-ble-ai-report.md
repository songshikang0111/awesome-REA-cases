# NEAR Signer: an AI-collaborative iPhone Ledger-protocol implementation, with hardware checks outstanding

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-12
Stage: In progress

At 13:01:43 Beijing time on November 12, 2026, Musin (@musinoot) describes near/near-signer-ios: an iPhone signing device for NEAR transactions and messages that uses the Ledger Nano X Bluetooth interface for existing near-connect and near-cli-rs hosts, with QR request/signature exchange as another channel. The article attributes development by Ivan Frolov and his agents to Vlad Frolov and mentions Claude code review. This is a concrete protocol-compatible implementation, not evidence that AI decompiled Ledger firmware or recovered original source. REA is not mentioned. Retrieving the same post supplied its full latter half; introductory promotion alone must not be treated as hardware validation.

Supplementary reading uses the README at commit c779108b128a47f9753edbd54131b0de6a352149, committed November 12 at 01:16:14 before the candidate. It documents NEAR Ledger APDUs and Nano X BLE framing, near-cli-rs 0.25 or newer, and near-connect through Chrome/Edge, with the app in the foreground. iOS cannot act as a USB Ledger; Safari/Firefox lack Web Bluetooth. My Ledger device management needs firmware details and a genuine-device check and cannot work. The README also describes QR transport, rejection of unknown or incompletely decoded requests, and approval after reviewing fields followed by Face ID or passcode unlocking.

Security must not be equated with a real Ledger: the Secure Enclave cannot hold the required ed25519 secret. The project encrypts it using a P-256 key and decrypts it into the app process for signing; the docs say it is neither backed up nor synced to iCloud. The README's verification section reports 128 Swift tests and 14 Python end-to-end tests passing on Linux, near-connect negotiation and signing over emulated BLE, matching near-cli-rs 0.30.1/simulator output, and QR codecs covered by 17 Node and 20 Rust tests. Loss simulations include 30% dropped/reordered frames and a 300 KB deployment with 20% loss, not an iPhone camera experiment.

The same section explicitly says there was no Mac or iPhone: real Xcode builds, screen appearance, Bluetooth radio pairing with macOS/Linux/Windows, phone scanning speed and real-camera response reading were not verified. Type checking against handwritten framework stand-ins does not replace an Apple SDK build. A documented Claude PR-review workflow is not an independent security audit. The candidate says users need Xcode 26 and iOS 17 or newer, with no App Store release; QR tool version 0.1.0 is not an iPhone app release. This collection built nothing, ran no tests, connected no wallet and signed no transactions. Status remains in progress and tests remain attributed to the project.

Sealed candidate: 0 likes, 313 views, 0 reposts. One star is the author's noon snapshot, not independently checked engagement.
All test counts are project reports in the pinned README; none were run here and they do not establish physical-device or funds security.

## Sources

- [Musin's NEAR Signer project account, November 12, 2026 at 13:01:43 Beijing time; full text retrieved from the same post](https://x.com/i/status/2120743823085281609)
- [Supplementary pinned NEAR Signer README committed November 12, 2026 at 01:16:14 Beijing time, before the candidate; protocol, security and verification scope](https://github.com/near/near-signer-ios/blob/c779108b128a47f9753edbd54131b0de6a352149/README.md)

[中文](../near-signer-ios-ledger-ble-ai-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
