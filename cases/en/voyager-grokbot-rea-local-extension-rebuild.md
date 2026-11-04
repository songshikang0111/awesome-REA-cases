# A local Voyager extension rebuild: five Grok Bot roles, static findings and an unresolved scrolling fault

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-05
Stage: In progress

From 00:19 Beijing time on November 5, 2026, Francesco Faenzi (@francescofaenzi) describes Grok Bot studying and locally rebuilding the Voyager Chrome extension to remove telemetry, cloud synchronization and broad permissions while retaining a local prompt panel. He calls the original open source and identifies version 2.2.1. A confirmed repository, license and payload were not obtained; his risk language does not establish maliciousness.

Five peer bots take Team Lead, Analyst, Spec Writer, Rebuilder and Verifier roles for static investigation, specifications, implementation and checks. He says the Analyst produces REA-evidence.md with 26 risks under an OAuth, Drive-sync and DOM-observer scope. The blueprint requires eliminating stored OAuth tokens, Google Drive background synchronization, MAIN-world observers and broad host permissions, and separating research, handoff, implementation and report directories. REA is also expanded as a Reverse Engineering Agent role family; actual use of morluto/rea is unconfirmed, so attribution is unknown, not a certified tool invocation.

Round one is called 97.5% successful, with cloud dependencies removed but the T29 folder-reordering UI missing. Operator testing then finds the local panel cannot scroll. The author attributes this to flexbox/overflow inheritance, yet round-two CSS changes still do not restore scrolling. The blueprint recommends further JavaScript/CSS overrides and a final PDF export, but candidates supply no actual third-round result, test inventory or final delivery. Requirements are not successes. The 26 are not independently confirmed vulnerabilities and 97.5% lacks a denominator and acceptance records. The extension and full audit artifacts were not run or inspected, and absence of telemetry was not verified. Localization alone establishes neither security nor legally clean-room implementation.

Sealed snapshots in source order: 0 likes/31 views, 0/4, 0/2, 0/3 and 0/10, all with 0 reposts. Architecture publicity is not runtime evidence.

## Sources

- [Faenzi's Voyager/Grok Bot opening post, November 5, 2026](https://x.com/i/status/2118015167586033749)
- [Same-thread peer-bot architecture](https://x.com/i/status/2118015193779511448)
- [Round-one static audit and claimed 97.5%](https://x.com/i/status/2118015254110363927)
- [Round-two scrolling fix still fails](https://x.com/i/status/2118015266131239248)
- [Same-thread rebuild blueprint and removal targets](https://x.com/i/status/2118015290550407647)

[中文](../voyager-grokbot-rea-local-extension-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
