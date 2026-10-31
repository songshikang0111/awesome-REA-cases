# Bastion: Claude router-privacy research leads to a bounded desktop network checker

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 03:37:43 Beijing time on October 31, 2026, an author says Claude reverse-engineered their Wi-Fi router, finding unencrypted DNS lookups visible to the ISP, then helped build Bastion. The post describes an Electron/Node Mac/Windows checker built by nine agents, each with a reviewer and fixer, totaling 27 agents, and checking 12 categories of entry points. Its first scan reportedly found SSH and UPnP enabled, 22 neighboring networks competing on the channel, and a 77/100 score. These are author reports. Observable unencrypted DNS does not mean an ISP actually stored all browsing history or decrypted HTTPS page content.

Earlier supplementary search located 0xCodez/bastion. Pinned commit 6fca59ba7a25c62875d1cf3a2b3892f33da23931 is dated 2026-10-30T19:28:26Z, or October 31 at 03:28:26 Beijing time, before both candidates. It supplements the project, not another candidate or a confirmed short-link destination. The README lists computer-side checks for TR-069/7547, UPnP, Telnet/SSH, HTTP administration, DNS, WPS and more, explicitly without password attempts, router login or exploits. LAN port responses do not prove internet reachability; it cannot see other devices' traffic, only local-computer connections and visible devices. Router APIs, external exposure checks and automatic fixes remain roadmap items.

The post claims 5–60-minute monitoring that wakes an agent only on changes; the README still lists scheduled watch as future work, so delivery is unconfirmed. Eleven fixed security issues are also claimed without an itemized acceptance report. The README describes Claude/ChatGPT subscriptions via already authenticated official CLIs, or user-supplied Claude/ChatGPT/Grok API keys. Agents only advise; users make changes. Plan limits and provider terms still apply: this is not offline AI.

This window's 05:14:56 long post adds reported hardware troubleshooting: Windows 11 required Location permission for Wi-Fi details; after a Cloudflare speed test hit HTTP 429, fewer, larger requests reportedly made the next run clean. It also claims CLIs run read-only with zero tools in an empty folder, questions travel through stdin, and Bastion refuses to start if Codex's shell tool is enabled. The author claims completion in one evening without personally writing code. These build/isolation claims have no hardware logs, itemized audit or adversarial tests here. Stdin argument handling alone does not prove injection is impossible, and the earlier README's watch-roadmap limitation remains.

The post claims MAC addresses, device names, Wi-Fi names and the last IP segment are stripped before sending. Documentation describes a privacy-minimized scan snapshot and discloses ipify, public speed testing and local-device PTR lookup boundaries. Without line-by-line source auditing or observed traffic, anonymity, no leakage and complete safety are not guaranteed. Windows builds are unsigned; macOS builds are ad-hoc signed and unnotarized. Screenshot and clone-address placeholders remain in the README; download links are not independent installation acceptance. Router model, firmware and recovered protocol details are unspecified, as is REA. This collection only read public material: no network scan, installation, CLI login or target-code execution occurred.

Original candidate snapshot: 29 likes, 810 views, 0 reposts. This window's candidate: 37 likes, 2,140 views, 3 reposts. Twenty-seven agents, 12 checks, 77/100, 22 neighboring networks and 11 fixes are post claims.
Pinned commit 2026-10-30T19:28:26Z predates this window. Scheduled watch remains future work in the README and is not independently confirmed.
One-evening completion, Windows permissions, the 429 fix and CLI isolation are author reports, not hardware acceptance testing by this collection.

## Sources

- [Author reports Claude router research and the Bastion build, October 31, 2026 at 03:37:43](https://x.com/i/status/2116253233308110936)
- [Supplementary: earlier pinned README, LAN observations, privacy and undelivered roadmap, October 31, 2026 at 03:28:26 Beijing time](https://github.com/0xCodez/bastion/blob/6fca59ba7a25c62875d1cf3a2b3892f33da23931/README.md)
- [This window's long post: Windows permissions, speed-test 429 and CLI-isolation claims, October 31, 2026 at 05:14:56](https://x.com/i/status/2116277697563234432)

[中文](../bastion-claude-router-privacy-network-guard-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
