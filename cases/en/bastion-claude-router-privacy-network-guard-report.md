# Bastion: Claude router-privacy research leads to a bounded desktop network checker

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 03:37:43 Beijing time on October 31, 2026, an author says Claude reverse-engineered their Wi-Fi router, finding unencrypted DNS lookups visible to the ISP, then helped build Bastion. The post describes an Electron/Node Mac/Windows checker built by nine agents, each with a reviewer and fixer, totaling 27 agents, and checking 12 categories of entry points. Its first scan reportedly found SSH and UPnP enabled, 22 neighboring networks competing on the channel, and a 77/100 score. These are author reports. Observable unencrypted DNS does not mean an ISP actually stored all browsing history or decrypted HTTPS page content.

Supplementary search located 0xCodez/bastion. Pinned commit 6fca59ba7a25c62875d1cf3a2b3892f33da23931 is dated 2026-10-30T19:28:26Z, inside the window before the candidate. It supplements the project, not another candidate or a confirmed short-link destination. The README lists computer-side checks for TR-069/7547, UPnP, Telnet/SSH, HTTP administration, DNS, WPS and more, explicitly without password attempts, router login or exploits. LAN port responses do not prove internet reachability; it cannot see other devices' traffic, only local-computer connections and visible devices. Router APIs, external exposure checks and automatic fixes remain roadmap items.

The post claims 5–60-minute monitoring that wakes an agent only on changes; the README still lists scheduled watch as future work, so delivery is unconfirmed. Eleven fixed security issues are also claimed without an itemized acceptance report. The README describes Claude/ChatGPT subscriptions via already authenticated official CLIs, or user-supplied Claude/ChatGPT/Grok API keys. Agents only advise; users make changes. Plan limits and provider terms still apply: this is not offline AI.

The post claims MAC addresses, device names, Wi-Fi names and the last IP segment are stripped before sending. Documentation describes a privacy-minimized scan snapshot and discloses ipify, public speed testing and local-device PTR lookup boundaries. Without line-by-line source auditing or observed traffic, anonymity, no leakage and complete safety are not guaranteed. Windows builds are unsigned; macOS builds are ad-hoc signed and unnotarized. Screenshot and clone-address placeholders remain in the README; download links are not independent installation acceptance. Router model, firmware and recovered protocol details are unspecified, as is REA. This collection only read public material: no network scan, installation, CLI login or target-code execution occurred.

Candidate snapshot: 29 likes, 810 views, 0 reposts. Twenty-seven agents, 12 checks, 77/100, 22 neighboring networks and 11 fixes are post claims.
Pinned commit 2026-10-30T19:28:26Z is within the window. Scheduled watch remains future work in the README and is not independently confirmed.

## Sources

- [Author reports Claude router research and the Bastion build, October 31, 2026 at 03:37:43](https://x.com/i/status/2116253233308110936)
- [Supplementary: earlier in-window pinned README, LAN observations, privacy and undelivered roadmap](https://github.com/0xCodez/bastion/blob/6fca59ba7a25c62875d1cf3a2b3892f33da23931/README.md)

[中文](../bastion-claude-router-privacy-network-guard-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
