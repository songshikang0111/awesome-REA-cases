# Reusing a SenseCAP M1: fan and button GPIO findings handed off to agents

Category: Hardware and interoperability · REA use unconfirmed
Record date: 2026-11-07
Stage: Related project

At 02:00:02 Beijing time on November 7, 2026, brainstormity (@brainstormity) reports repurposing a SenseCAP M1 LoRaWAN gateway. The author claims a new sealed unit cost $62 and contains a quad-core Raspberry Pi 4B, 8GB RAM, a 64GB high-endurance SD card, WM1302 LoRaWAN module, metal case, 5V 3A supply, fan/heatsink, antenna, security element and button, recommending reuse intact instead of removing only the Pi.

After switching to Raspberry Pi OS, the fan and button reportedly do not work by default. The author says reverse engineering identified fan GPIO13 and button GPIO27 for boot/temperature-controlled fan behavior and custom button actions, and offers a Markdown file to assist AI agents. This establishes an agent handoff for findings, not AI participation in original pin discovery; REA or automatic AI reversing is not claimed. Retrieval confirms attribution, not the document's short-link contents.

Monthly electricity of $0.90, stress temperatures below 52°C and component value above $300 are author claims without power measurements, ambient temperature, test duration or price checks. A 1–3-mile sensor security system on US 915/EU 868MHz is a future use idea, not a demonstrated LoRa deployment. Hardware revisions, electrical safety, stock-system recovery and full peripheral support are untested. No card was flashed, device connected, agent document executed or GPIO tested here. Kept as a related hardware-interoperability project.

Sealed snapshot: 7 likes, 498 views, 0 reposts. $62, $0.90/month, 52°C and GPIO mappings are author reports, not measurements here.

## Sources

- [brainstormity's SenseCAP M1 reuse, GPIO and agent-document report, November 7, 2026 at 02:00:02 Beijing time](https://x.com/i/status/2118765365123567760)

[中文](../sensecap-m1-gpio-fan-button-agent-repurpose.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
