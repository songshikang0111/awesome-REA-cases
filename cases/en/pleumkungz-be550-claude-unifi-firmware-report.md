# TP-Link BE550: Pleumkungz reports Claude-modified stock firmware with a UniFi agent and a successful flash

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-21
Stage: Needs verification

At 14:24:29 Beijing time on November 21, 2026, Pleumkungz (@pleumkungz_t) reports a router-firmware modification in Thai. To avoid buying another wireless access point (AP), the author first tried porting U7 Pro OpenWrt firmware to a BE550. Opening the device was difficult, and reaching the UART serial interface might require damaging the enclosure. The author therefore switched to modifying TP-Link stock firmware rather than continuing that port.

The post explicitly names Claude Mythos 5.2 for modifying the firmware, adding unifi agent and making fakectrl, and says flashing succeeded. Component names and the model label are preserved as written. The role or implementation of fakectrl is not independently established, and the initial OpenWrt port is not presented as completed. The concrete goal is to repurpose the existing BE550 for the desired AP/UniFi-related functionality. Modifying existing firmware for interoperability fits the broader AI-assisted reverse-engineering scope, but the post describes no disassembly, protocol analysis or REA invocation.

Retrieving the original confirms attribution and the complete wording. No hardware revision, firmware version, source, patch, controller version, runtime logs, networking demonstration or recovery test is supplied. Successful flashing is only an author-reported intermediate result: it does not establish a normal boot, adoption by a UniFi controller, wireless functionality, upgrade compatibility or long-term stability. Equivalence to a U7 Pro cannot be inferred. This collection accessed no device, downloaded no firmware, executed no project and did not verify component provenance; no flashing procedure is provided. Status remains unverified with the author-report boundary intact.

November 21 sealed candidate snapshot: 0 likes, 11 views, 0 reposts, 0 replies. Engagement is not firmware or interoperability validation.
The only outcome is the author's successful-flash report. No boot, controller-adoption or networking test was obtained; not independently reproduced.

## Sources

- [Pleumkungz's BE550 firmware-modification and flashing report, November 21, 2026 at 14:24:29 Beijing time](https://x.com/i/status/2124026142160245105)

[中文](../pleumkungz-be550-claude-unifi-firmware-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
