# Per-device OpenWrt gateways: Codex rebuilds an ASUS-style configuration workflow

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-20
Stage: Needs verification

At 21:36 Beijing time on November 20, 2026, xiaojingshe (@xiaojingshe) says manual per-device gateway tags and bindings in OpenWrt are cumbersome. Codex reportedly used ASUS's custom-gateway design as a reference for a plugin where users select a device, gateway and DNS and save. What is reconstructed is an interaction workflow, not a claimed ASUS firmware decompilation or private-protocol discovery.

The short link identifies huladabang/luci-app-device-gateway. Supplementary reading used README at the pre-candidate commit c593d0d4407dfa4505bf055afa01082ce1af682c, November 20 at 12:37:02 Beijing time. It describes LuCI rules saved to UCI and scripts maintaining dnsmasq DHCPv4 tags, Option 3 gateways and Option 6 DNS; clients must renew leases. The plugin does not provide the side router's forwarding, firewall or IPv6 RA.

The project reports an r20 functional check only on a TP-Link TL-7DR7299 with ImmortalWrt 24.10-SNAPSHOT and LuCI 24.10. Other official 24.10 systems are offered for trials; 23.05/22.03 need integrated tests. Official 25.12 uses apk and cannot directly install the existing IPK; the package also omits a declared flock dependency. Documented recovery attempts are not safety guarantees. Only public docs were read here: no package, script or router was run, and a single-device report is not generalized. REA is not mentioned.

Sealed snapshot: 54 likes, 5,254 views, 6 reposts, 11 replies. Single-device validation and compatibility scope are project documentation, not rerun here.

## Sources

- [xiaojingshe introduces the Codex gateway plugin, November 20, 2026 at 21:36 Beijing time](https://x.com/i/status/2123772350277812717)
- [Supplement: pinned pre-candidate README, November 20, 2026 at 12:37:02 Beijing time](https://github.com/huladabang/luci-app-device-gateway/blob/c593d0d4407dfa4505bf055afa01082ce1af682c/README.md)

[中文](../openwrt-codex-asus-gateway-workflow-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
